# configure third-party loans

use Third-Party Loans for a company-supported lender or loan that is not part of the government-loan workflow. Define the loan type by its name and description first, then assign the employee's loan balance and amortization terms.

**navigation:** for setup, go to **Settings → Paycheck → Deductions → Third-Party Loans**. for assignment, go to **Workforce → Third-Party Deductions** or the current Third-Party Loans page.

## how is this different from a government loan?

Government Loans uses the supported SSS and HDMF loan types and a government-loan remittance workflow. Third-Party Loans uses company-defined loan types and stores the employee's total payable amount and amortization terms.

do not use Other Deductions as a substitute when the item needs a loan number, payable balance, payment count, amortization, or loan status.

## how do i create a third-party loan type?

1. open **Settings → Paycheck → Deductions → Third-Party Loans**.
2. select **Add Third Party Loans**.
3. enter the loan type name and description.
4. review whether an equivalent type already exists.
5. save the loan type.

the setting makes the type available for assignment; it does not create an employee balance.

## short-term and long-term assignment modes

the current employee workflow can expose short-term and long-term assignment modes.

| mode       | typical controls                                                                                    |
| ---------- | --------------------------------------------------------------------------------------------------- |
| short term | manual or fixed amortization, payroll schedule, start/end dates, and calculated amortization amount |
| long term  | entered amortization amount, first remittance date, number of payments, and payroll schedule        |

use the mode shown by the employee page and the approved loan agreement. Do not choose a mode only to bypass required dates or payment-count controls.

## how do i assign a third-party loan?

1. open the Third-Party Loans employee page.
2. select **Assign 3P Loan** and choose the available short-term or long-term option.
3. Search for and select the employee.
4. select the loan type.
5. enter the loan number and description.
6. enter the **Total Payable Loan Amount**.
7. for short-term fixed amortization:
   * select the payroll schedule;
   * enter start and end dates; and
   * select **Calculate** to obtain the amortization amount.
8. for a manually added short-term schedule, confirm the manually supplied amortization information.
9. for long-term treatment:
   * enter the amortization amount;
   * enter the first remittance date;
   * enter the number of payments; and
   * select the payroll schedule.
10. review the total, amortization, schedule, and dates.
11. save the loan.
12. Recalculate and review the affected open payroll.

## how do i pause, complete, correct, or delete a loan?

Additional schedules require an ongoing loan with a positive remaining balance and dates that match the employee payroll calendar. When a selected bulk-amortization range has no matching rows, Ashima reports that no matches were found. When matching rows exist but all of them are already processed or belong to closed payroll, Ashima reports that those rows cannot be edited. Use the filtered CSV download to review the current loan scope.

the list supports status review, including active, paused, and completed records.

* Pause only when deductions should temporarily stop without changing the loan's business identity.
* complete the loan when the approved payable obligation has been satisfied.
* Correct an editable active record when the loan itself is unchanged.
* create a separate loan when it is an intentionally different obligation with its own loan number and terms.
* Delete only an eligible erroneous record after checking open payroll and history.

## what should i review after saving?

* employee and loan type;
* loan number;
* total payable amount;
* amortization method and amount;
* first remittance or start date;
* end date or number of payments;
* payment schedule and employee payroll calendar;
* status and remaining obligation; and
* affected open payroll, payslip, and payroll reports.

## downloads and troubleshooting

the list provides Excel and CSV downloads. Apply the intended employee, loan, or status filters and verify the downloaded scope.

* **No loan type is available:** create or review the correct loan type.
* **Unable to calculate amortization:** review total payable amount, dates, schedule, and employee payroll calendar.
* **Loan continued after intended stop:** review status, end date or number of payments, and remaining balance.
* **Possible duplicate:** compare employee, loan type, loan number, and active obligation before adding another record.
* a completed-payroll deduction is not reversed by deleting the current loan record.

## continue in the affected module

* [review third-party loans in payroll](../../paycheck/)
