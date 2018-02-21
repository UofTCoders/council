
Documentation for the Treasurer
===============================

Keep all transactions (income and expenses) in the `accounting.csv` file, with the date in the ISO 8601 standard format (*YYYY-MM-DD*, all numbers). Income in the `Income` column, expenses in the `Expense` column. When recording the incomes and expenses in the `accounting.csv` file, for cheques include the date that you wrote the cheque up in the `TransactionDate` column. Once in a while, compare the transaction dates in the BMO online account with the `accounting.csv` date. If they are different, update the date using the BMO online account. Ultimately, the goal is that the BMO accounting and the GitHub accounting should be the same.

Receipts should be scanned and placed in the `receipts/` folder, with the filename as the ISO 8601 date format (`YYYY-MM-DD`), followed by the item and then the location of purchase. For instance, food purchased on June 5, 2000 would be `2000-06-05-Snacks-Loblaws.pdf`.

Record the relevant details about cheques given out in the `cheques/` folder in the `cheques.csv` file. Fill in the appropriate columns. Take a picture of the cheque with the signatures and save that cheque in the `cheques/images/` folder. *Important*, **do not** commit these cheque images in the Git repository. They should not be publicly viewable. Git ignores all files in the `cheques/images/` folder.

Given that this is a *coders* group, all summaries of the finances are done in R with R Markdown. *Occasionally* this document will need to be re-knitted to reflect an accurate portrayal of the financial situation of the UofTCoders.

Accounting overview
===================

All calculations were performed using R. For the code, please see the `README.Rmd` file.

Actual income and expenses
--------------------------

| Type      | Amount    |
|:----------|:----------|
| Income    | $4,362.85 |
| Expense   | $3,507.98 |
| **Total** | $854.87   |

    ## Warning in grepl("Snacks", Reason): input string 25 is invalid in this
    ## locale

**Per session (weekly) expense for snacks**: $5.32

Projected income and expenses
-----------------------------

Values surrounded by brackets `()` denote negative values, as is often done in accounting. Projected values are until end of *fiscal year*. Fiscal year starts from the month we first started using the BMO bank account (May):

Fiscal year: *May 1st-April 30th.*

    ## Warning in grepl("walk-in", Reason): input string 25 is invalid in this
    ## locale

    ## Warning: package 'pander' was built under R version 3.2.5

| Item      |       Amount|
|:----------|------------:|
| Snacks    |     ($52.49)|
| Misc      |       ($200)|
| Workshops |      $727.88|
| **Total** |  **$475.39**|
