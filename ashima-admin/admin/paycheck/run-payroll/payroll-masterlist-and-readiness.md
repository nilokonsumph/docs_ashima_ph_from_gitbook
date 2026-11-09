# Payroll masterlist and readiness

Use Payroll Masterlist to review consolidated employee payroll, check for source updates, prepare employee pay drafts, and submit a ready payroll for approval.

**Navigation:**\
open **View Payroll Masterlist** from Pay Run, or select **continue to masterlist** from Pay Run Details.

## before you begin

* verify the status, Pay Run IDs, pay date, period from/to, and total net pay.
* recalculate after eligible source changes.
* review exclusions, direct adjustments, and employee-level outliers.
* confirm the payroll approval workflow and payroll lock state.

## which settings control this workflow?

| level            | setting or record                                                                 | effect                                                              |
| ---------------- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| company / global | payroll, payment, payslip, workflow, and output settings                          | controls reusable payroll review and release behavior               |
| module           | readiness checks, pay-update detection, approval, payroll lock, and output rules  | controls whether the run can proceed and what actions are available |
| employee         | calculated payroll result and employee delivery/payment details                   | supplies each row and related output data                           |
| pay run          | selected Pay Run IDs, dates, status, exclusions, adjustments, and pay-draft state | defines the consolidated review and submission                      |

## what does the page show?

The current table shows Employee Details, Payroll Group, Total Gross Pay, Total Taxable Pay, Total Non Taxable Pay, Total Withholding Tax, Total Deductions, and Net Pay. Select an employee's Net Pay to open Employee Pay Details.

The page also exposes **paycheck adjustment**, **exclusion**, employee search, download, **Check for Pay Updates**, **Send Pay Draft**, and **Submit for Approval** when available.

## how do you review readiness?

1. confirm the Pay Run IDs and summary dates.
2. review totals and investigate zero, negative, or unusual values.
3. select **Check for Pay Updates**.
4. review employees identified as having updates affecting timesheets, shifts/settings, or pay items.
5. return to the appropriate source workflow and recalculate before submission.
6. review the P and T indicators, but do not rely on color alone; use the employee/update details provided by the page.
7. generate or review the required download and pay-draft outputs.
8. submit only when the page enables **Submit for Approval** and all identified updates are resolved.

## recalculation prompt when continuing

When continuing from Pay Run Details, the current page asks whether to recalculate before opening the masterlist. **Good idea. Recalculate before continuing to masterlist** runs recalculation; **No Need. Skip Recalculation** continues without it. Skip only when you have confirmed that no eligible source inputs changed after the last successful recalculation.

> \[!WARNING] Sending a Pay Draft is a preview/delivery action. It does not approve or close payroll. Submitting for approval changes the payroll state and should happen only after the complete masterlist and readiness checks pass.

## related articles

* [employee pay details](/broken/pages/fc19fcc831aa20c240ee9f0cde597b7cb8a4c2ea)
* [review and recalculate a pay run](/broken/pages/4b2260817fafa8f67821e1a140643d4dd7a297ab)
* [pay run workspace and history](/broken/pages/1aae811cf00a844c563a72b274efd3a4f11bcde1)
