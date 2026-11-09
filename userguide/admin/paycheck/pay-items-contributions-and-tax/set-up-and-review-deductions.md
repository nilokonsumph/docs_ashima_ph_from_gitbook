# set up and review deductions

## set up and review deductions

### what is the normal deductions workflow?

Most deduction groups also start with a company setup, but not all of them follow the same pattern.

There are two main models:

1. reusable deduction types created in **Settings**, then assigned to employees
2. payroll-rule deductions that are computed from company rules plus employee payroll information

### which deductions are reusable types and which are payroll-rule outputs?

* **Reusable deduction types:** **Government Loans**, **Third Party Loans**, **Insurance**, **Other Deductions**
* **Payroll-rule outputs:** **Contributions**, **Withholding Tax**

### how do deductions move from setup to payroll output?

| Deduction group       | Setup pattern                                               | Global setup page                                        | What the global setup controls                                                          | What the employee-level record controls                                                                         | How it appears in admin payroll review                                                  | How it appears in masterlist or download                                                                          | How it appears on the payslip                                                                      |
| --------------------- | ----------------------------------------------------------- | -------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **Government Loans**  | Reusable deduction type, then assigned to employees         | **Settings → Paycheck → Deductions → Government Loans**  | Loan type name and which employee groups it can apply to                                | Employee loan record, amount, schedule, start or end timing, active deduction row                               | Reviewed under the broader **Loans** section, then folded into deduction totals         | Masterlist page: inside totals only. Masterlist download can break out government-loan types into report columns  | Shown under **Loans** with government-loan detail rows                                             |
| **Third Party Loans** | Reusable deduction type, then assigned to employees         | **Settings → Paycheck → Deductions → Third Party Loans** | Loan type name and base description                                                     | Employee loan number, amortization or installment amount, schedule, active deduction row                        | Reviewed under the broader **Loans** section, then folded into deduction totals         | Masterlist page: inside totals only. Masterlist download can break out third-party-loan types into report columns | Shown under **Loans** with third-party-loan detail rows                                            |
| **Insurance**         | Reusable deduction type, then assigned to employees         | **Settings → Paycheck → Deductions → Insurance**         | Provider or insurance type, default deduction logic, recurrence, schedule, plan details | Employee amount, active deduction row, employee-level tax-exempt handling where used                            | Reviewed as its own **Insurance** deduction block                                       | Masterlist page: inside totals only. Masterlist download can break out insurance types into report columns        | Shown as its own **Insurance** deduction group                                                     |
| **Other Deductions**  | Reusable deduction type, then assigned to employees         | **Settings → Paycheck → Deductions → Other Deductions**  | Deduction name, description, recurrence, schedule, default amount, applicability        | Employee amount, active deduction row, employee-specific release or recurrence details                          | Reviewed as its own **Other Deductions** block                                          | Masterlist page: inside totals only. Masterlist download can break out other-deduction types into report columns  | Shown as its own **Other Deductions** group                                                        |
| **Contributions**     | Payroll-rule output, not a reusable assigned deduction type | **Settings → Paycheck → Contribution** pages             | Company contribution rules, tables, schedules, and calculation behavior                 | Employee entitlement, employee contribution mode, custom or fixed contribution behavior, employee payroll flags | Reviewed as computed payroll deductions, not as reusable deduction rows                 | Reported as standard payroll contribution columns, not as user-selected deduction types                           | Shown as top-level contribution lines such as **SSS**, **PHIC**, **HDMF**, **HDMF I**, **HDMF II** |
| **Withholding Tax**   | Payroll-rule output, not a reusable assigned deduction type | **Settings → Paycheck → Taxes → Withholding Tax** pages  | Tax rules and withholding-tax computation behavior                                      | Employee tax status and payroll tax profile; separate tax-adjustment tools may also affect final output         | Reviewed as computed tax output, including tax adjustment or fixed-tax lines where used | Reported as standard payroll tax columns, not as a reusable deduction family                                      | Shown as top-level **withholding tax** and fixed-tax lines where applicable                        |

### what fields usually come from the deduction setup?

For reusable deduction types, the global setup usually defines:

* deduction or loan type name
* schedule logic
* recurrence logic
* default amount behavior
* applicability to employee groups

### what fields are usually controlled at employee level?

For reusable deduction types, the employee-level record usually controls:

* which employee receives the deduction
* the actual deduction amount or installment
* start and end timing
* pay status or active status
* employee-specific schedule details

This is why the company can reuse one deduction type across many employees while still carrying different employee-level amounts or schedules.

### what should administrators know about Government Loans and Third Party Loans?

Both of these are reusable loan types created first in **Settings**, then assigned through employee loan records.

The important presentation rule is:

* they are set up separately
* they remain separate data families in payroll
* but paycheck review and payslip display group them together under **Loans**

So an admin may create or assign them differently, but still review them together later in payroll output.

### what should administrators know about Insurance?

Insurance is a reusable deduction type with more payroll detail than a simple flat deduction.

The company setup can define:

* provider or insurance type
* deduction amount
* recurrence
* schedule
* plan-related details

The employee-level record then carries the actual active deduction row for that employee.

In payroll review, insurance appears as its own deduction block rather than being merged into loans or other deductions.

### what should administrators know about Other Deductions?

Other Deductions are reusable deduction types created in **Settings**, then assigned to employees.

Use this when the deduction should remain its own named deduction type rather than being treated as a loan, insurance item, or statutory contribution.

In payroll review:

* it appears as its own **Other Deductions** block
* it is included in deduction totals on the masterlist page
* selected downloads can still break it out by deduction type
