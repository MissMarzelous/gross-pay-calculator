# PROGRAMMER:   Marlena Fabrick
# PROGRAM NAME: Gross Pay Calculator
# DATE WRITTEN: 9/8/2020
# UPDATED:      2026 — added input validation, f-strings, fixed typos in comments
#
# PURPOSE: Calculate the gross pay for an employee given their name,
#          hours worked, and hourly pay rate. Displays a formatted payroll report.
#
# BEFORE (original): Used string concatenation and toFixed() helper function.
#                    Had typos: "employess's" and "proceessed".
# AFTER  (improved): Uses f-strings for cleaner output, added try/except
#                    for invalid input, fixed all comment typos.

# ============================================================
# Declare variables
# Initialize processed variable
gross_pay = 0.0

# ============================================================
# Input Operations — collect employee info from the user

print("Enter the employee's full name:")
employee_name = input()

# Loop until valid numeric input is provided for hours worked
while True:
    try:
        print(f"How many hours did {employee_name} work?")
        hours_worked = float(input())
        break  # Exit loop once a valid number is entered
    except ValueError:
        print("Invalid input. Please enter a numeric value for hours worked.")

# Loop until valid numeric input is provided for pay rate
while True:
    try:
        print(f"What is the hourly rate of pay for {employee_name}?")
        pay_rate = float(input())
        break  # Exit loop once a valid number is entered
    except ValueError:
        print("Invalid input. Please enter a numeric value for pay rate.")

# ============================================================
# Calculate Gross Pay
gross_pay = hours_worked * pay_rate

# ============================================================
# Output Operations — display formatted payroll report
print("================================================================")
print(f"PAYROLL INFORMATION FOR: {employee_name}")
print(f" Hours Worked =   {format(hours_worked, '11,.2f')}")
print(f"  Rate of Pay = $ {format(pay_rate,     '11,.2f')}")
print(f"    Gross Pay = $ {format(gross_pay,    '11,.2f')}")
print("================================================================")

# END PROGRAM
