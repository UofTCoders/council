Documentation for the Treasurer
===============================

Keep all transactions (income and expenses) in the `accounting.csv` file, with the date in the ISO 8601 standard format (*YYYY-MM-DD*, all numbers). Income should be positive, expenses should be negative (with a minus `-` sign in front).

Receipts should be scanned and placed in the `receipts/` folder, with the filename as the general item first followed by the ISO 8601 date format. For instance, food purchased on June 5, 2000 would be `food-2000-06-05.pdf`.

Given that this is a *coders* group, all summaries of the finances are done in R with R Markdown. Code is included in the output.

Accounting overview
===================

``` r
# Load the packages and data.
library(dplyr)
library(tidyr)
library(pander)
finances <- read.csv('accounting.csv') %>% 
    mutate(Date = lubridate::ymd(Date))
```

Actual income and expenses
--------------------------

**Total funds remaining**: $709.26

``` r
finances %>% 
    mutate(Type = ifelse(Transaction < 0, 'Expense', 'Income')) %>% 
    group_by(Type) %>% 
    summarise(Amount = sum(Transaction)) %>% 
    arrange(desc(Type)) %>% 
    knitr::kable()
```

| Type    |   Amount|
|:--------|--------:|
| Income  |  1700.00|
| Expense |  -990.74|

``` r
perWeekExpense <- finances %>% 
    filter(Transaction < 0, grepl('Snacks', Reason)) %>% {
        NumberWeeks <- as.numeric(difftime(Sys.Date(), min(.$Date), units = 'weeks'))
        PerWeekExpense <- sum(.$Transaction) / NumberWeeks
        abs(round(PerWeekExpense, 2))
    }
```

<!-- there are still 13.35 left in Luke's account -->
**Per session (weekly) expense**: $6.12

Projected income and expenses
-----------------------------

``` r
numWeeksLeftFiscalYear <- as.numeric(difftime('2017-03-31', Sys.Date(), units = 'weeks'))
estimatedBudget <- 
    data.frame(
        IncomeSWC = sum(c(600.60)),
        FoodSWC = -sum(c(112*2+75)),
        ## Not all weeks will there be a meet up (e.g. Christmas, random weeks).
        CodersSnacks = -perWeekExpense * (numWeeksLeftFiscalYear - 3 - 2)
    ) %>%
    mutate(Total = rowSums(.)) %>%
    gather(Item, Amount)

pander(estimatedBudget, emphasize.strong.rows = nrow(estimatedBudget), 
       style = 'rmarkdown', justify = c('left', 'right'))
```

| Item         |     Amount|
|:-------------|----------:|
| IncomeSWC    |      600.6|
| FoodSWC      |       -299|
| CodersSnacks |     -246.7|
| **Total**    |  **54.91**|
