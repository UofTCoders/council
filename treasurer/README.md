
Documentation for the Treasurer
===============================

Keep all transactions (income and expenses) in the `accounting.csv` file, with the date in the ISO 8601 standard format (*YYYY-MM-DD*, all numbers). Income should be positive, expenses should be negative (with a minus `-` sign in front).

Receipts should be scanned and placed in the `receipts/` folder, with the filename as the ISO 8601 date format (`YYYY-MM-DD`), followed by the item and then the location of purchase. For instance, food purchased on June 5, 2000 would be `2000-06-05-food-place.pdf`.

Given that this is a *coders* group, all summaries of the finances are done in R with R Markdown. Code is included in the output.

Accounting overview
===================

All calculations were performed using R. For the code, please see the `README.Rmd` file.

Actual income and expenses
--------------------------

| Type      | Amount    |
|:----------|:----------|
| Income    | $4,362.85 |
| Expense   | $3,347.83 |
| **Total** | $1,015.02 |

**Per session (weekly) expense for snacks**: $5.76

Projected income and expenses
-----------------------------

Values surrounded by brackets `()` denote negative values, as is often done in accounting. Projected values are until end of *fiscal year*. Fiscal year starts from the month we first started using the BMO bank account (May):

Fiscal year: *May 1st-April 30th.*

| Item      |       Amount|
|:----------|------------:|
| Snacks    |    ($102.91)|
| Misc      |       ($200)|
| Workshops |      $727.88|
| **Total** |  **$424.97**|
