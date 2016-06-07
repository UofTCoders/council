Documentation for the Treasurer
===============================

Keep all transactions (income and expenses) in the `accounting.csv` file, with the date in the ISO 8601 standard format (*YYYY-MM-DD*, all numbers). Income should be positive, expenses should be negative (with a minus `-` sign in front).

Receipts should be scanned and placed in the `receipts/` folder, with the filename as the ISO 8601 date format (`YYYY-MM-DD`), followed by the item and then the location of purchase. For instance, food purchased on June 5, 2000 would be `2000-06-05-food-place.pdf`.

Given that this is a *coders* group, all summaries of the finances are done in R with R Markdown. Code is included in the output.

Accounting overview
===================

``` r
# Load the packages and data.
library(dplyr)
library(tidyr)
library(pander)
library(lubridate)
library(scales)
cad <- dollar_format(negative_parens = TRUE)
finances <- read.csv('accounting.csv') %>% 
    mutate(Date = ymd(Date))
```

Actual income and expenses
--------------------------

``` r
finances %>%
    mutate(Type = ifelse(Transaction < 0, 'Expense', 'Income')) %>%
    group_by(Type) %>%
    summarise(Amount = cad(sum(Transaction))) %>%
    ungroup() %>%
    arrange(desc(Type)) %>%
    bind_rows(summarize(finances,
                        Type = '**Total remaining**',
                        Amount = cad(sum(Transaction)))) %>%
    knitr::kable()
```

| Type                | Amount      |
|:--------------------|:------------|
| Income              | $2,464.40   |
| Expense             | ($1,236.03) |
| **Total remaining** | $1,228.37   |

``` r
perWeekExpense <- finances %>% 
    filter(Transaction < 0, grepl('Snacks', Reason)) %>% {
        NumberWeeks <- as.numeric(difftime(Sys.Date(), min(.$Date), units = 'weeks'))
        abs(sum(.$Transaction) / NumberWeeks)
    }
```

<!-- there are still 13.35 left in Luke's account -->
**Per session (weekly) expense**: $7.68

Projected income and expenses
-----------------------------

``` r
numWeeksLeftFiscalYear <- as.numeric(difftime('2017-03-31', Sys.Date(), units = 'weeks'))
estimatedBudget <- 
    data.frame(
        ## Not all weeks will there be a meet up (e.g. Christmas, random weeks).
        CodersSnacks = -perWeekExpense * (numWeeksLeftFiscalYear - 3 - 2)
    ) %>%
    mutate(Total = rowSums(.)) %>%
    mutate_each(funs(cad)) %>% 
    gather(Item, Amount)

pander(estimatedBudget, emphasize.strong.rows = nrow(estimatedBudget), 
       style = 'rmarkdown', justify = c('left', 'right'))
```

| Item         |         Amount|
|:-------------|--------------:|
| CodersSnacks |      ($287.60)|
| **Total**    |  **($287.60)**|
