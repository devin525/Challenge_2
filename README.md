# Loan App additional features/ Challenge 2# Project Title

The user needs the ability to save the qualifying loans to a CSV file so that the results can be shared as a spreadsheet.
---

## Technologies
JupyterLabs 3.2.1
fire
questionary

---

## Installation Guide

Python Fire will run our funtion. We do this by using the __main__ declaration.
 
if __name__ == "__main__":
    fire.Fire(run)


---

## Usage

This is the main function for running the script.

def run():

    # Load the latest Bank data
    bank_data = load_bank_data()

    # Get the applicant's information
    credit_score, debt, income, loan_amount, home_value = get_applicant_info()

    # Find qualifying loans
    qualifying_loans = find_qualifying_loans(
        bank_data, credit_score, debt, income, loan_amount, home_value
    )

    # Save qualifying loans
    save_qualifying_loans(qualifying_loans)
---

## Contributors
Duvall, Devin 
dduvall525@gmail.com
---
