# **Loan Qualifier Application**



This is a **command line application** to match applicants with qualifying loans.

---

## Technologies

Python

- import sys

- from tkinter.messagebox import YES

- import fire

- import questionary

- from pathlib import Path

- from qualifier.utils.fileio import (load_csv, save_csv) *for both functions to run must import csv file within appropriate file*

- from qualifier.utils.calculators import (
    calculate_monthly_debt_ratio,
    calculate_loan_to_value_ratio,

- from qualifier.filters.max_loan_size import filter_max_loan_size
from qualifier.filters.credit_score import filter_credit_score
from qualifier.filters.debt_to_income import filter_debt_to_income
from qualifier.filters.loan_to_value import filter_loan_to_value


---

## Installation Guide

- `import sys`

- `from tkinter.messagebox import YES`

- `import fire`

- `import questionary`

- `import pathlib import Path`

- `from qualifier.utils.fileio import (load_csv, save_csv)`

- `from qualifier.utils.calculators import (calculate_monthly_debt_ratio,  calculate_loan_to_value_ratio)`

- `from qualifier.filters.max_loan_size import filter_max_loan_size`

- `from qualifier.filters.credit_score import filter_credit_score`

- `from qualifier.filters.debt_to_income import filter_debt_to_income`

- `from qualifier.filters.loan_to_value import filter_loan_to_value`

---

## Usage

This program asks the applicant 5 questions to obtain `credit_score`, `debt`, `income`, `loan_amount`, and `home_value`

Once the user inputs their data the program will calculate their monthly debt to income ratio and their loan to value ratio.

The program uses these criteria to filter the daily_rate_sheet only for loand the applicant qualifies for.

![alt text](screenshot_app.py.png\screenshot_app.py.png)

---

## Contributors

Severo Fernandez

severocf@gmail.com


---

## License

[MIT]