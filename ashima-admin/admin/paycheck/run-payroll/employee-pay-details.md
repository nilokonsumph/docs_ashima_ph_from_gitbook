# Employee pay details

Use Employee Pay Details to trace one employee's calculated payroll components before the payroll is submitted or closed.

**Navigation:**\
open an employee's Net Pay from **Pay Run Details** or **Payroll Masterlist**.

## before you begin

* confirm the employee, Pay Run ID, period from/to, pay date, and latest recalculation time.
* confirm whether payroll inputs changed after the displayed recalculation.
* investigate unexpected zero, negative, or unusually large values before proceeding.

## which settings control this workflow?

| level            | setting or record                                                                            | effect                                                     |
| ---------------- | -------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| company / global | pay rates, earnings/deductions, contribution, tax, time, leave, and premium settings         | provides reusable rules and item behavior                  |
| module           | payroll calculation, approval, lock, and adjustment rules                                    | determines eligible inputs and whether changes can be made |
| employee         | compensation, pay type, schedule, tax/contribution profile, entitlements, and assigned items | supplies employee-specific inputs                          |
| pay run          | period, pay date, exclusions, adjustments, ingestion, and last recalculation                 | produces the displayed employee result                     |

## what does the page show?

The summary displays Basic Pay, Hourly Rate, and Net Pay. The current earnings breakdown includes Regular Hours, Paid/Unpaid Leave, Overtime, Rest Day/Holiday, Night Shift Differential, Retroactive Pay, Post Payroll Adjustments, Adjustments, Allowances, De Minimis, Other Earnings, Withholding Tax adjustments, and Ingestion when applicable.

The deductions breakdown includes withholding tax, SSS, HDMF, PhilHealth, HDMF I/II, Insurance, Loans, Other Deductions, Other Adjustments, Boost, fixed withholding tax, and deduction-side Ingestion when applicable.

## how do you investigate an amount?

1. read the recalculation notice and confirm the pay-run dates.
2. compare Basic Pay, Total Earnings, Total Deductions, and Net Pay.
3. open a linked component to inspect its dated or source-level details.
4. use the withholding-tax breakdown action when tax requires explanation.
5. use **Withholding Tax (Adj)** or **paycheck ingestion** only for an authorized run-specific correction.
6. click **Recalc** after an eligible source record changes, then verify the complete result again.

> \[!WARNING] A component shown as `0.00` means no amount is currently included in that displayed payroll result. It does not prove that the employee lacks the related assignment or that the source module has no record.

## related articles

* [review and recalculate a pay run](/broken/pages/4b2260817fafa8f67821e1a140643d4dd7a297ab)
* [payroll masterlist and readiness](/broken/pages/90993c9dd2e7045a5799c0b820706e27adc169e8)
* [contribution settings](file:///4659123/settings/contribution_settings.md)
* [timesheet logs](file:///4659123/hours/timesheet_logs.md)
