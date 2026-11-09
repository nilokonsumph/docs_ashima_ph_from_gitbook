# Contribution

Contributions are payroll-calculated results, not reusable deduction rows assigned one employee at a time. The admin's job is to keep three things aligned:

* the company contribution rules
* the company contribution schedule
* the employee's contribution entitlement and mode

When those three are aligned, payroll calculates the contribution lines that appear in payroll review, reports, and the payslip.Contributions

Use the **Contribution** pages to review statutory contribution amounts, remittance details, and contribution rules used by payroll.

#### What are the three company contribution settings?

The admin’s job is to keep three things aligned:

* **Contribution Calculation** — which contribution methods are allowed for SSS, PhilHealth, and HDMF. Examples: SSS Contribution Table, SSS Fixed Rate, PhilHealth Contribution Table, PhilHealth Fixed Rate, HDMF Fixed 100, HDMF % of Base Pay, HDMF Mixed Deduction, HDMF Voluntary Increase, HDMF Modified.
* **Contribution Schedule** — when each contribution is deducted in the payroll month: first payroll, second payroll, every payroll, or last payroll of the month.
* **Contribution Rules** — which pay items count toward contribution basis: basic pay, selected earnings, and selected payroll adjustments.

When those three pieces line up, payroll calculates the contribution lines that appear later in review, reports, and the payslip.

#### How do the main contribution types work?

| Contribution                  | Company settings that drive it            | Employee-level controls                                                | What payroll shows                       |
| ----------------------------- | ----------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------- |
| **SSS**                       | Contribution Calculation, Schedule, Rules | Entitled to SSS, SSS mode (table or fixed), fixed amount where used    | Computed SSS deduction line              |
| **PhilHealth**                | Contribution Calculation, Schedule, Rules | Entitled to PhilHealth, mode (table or fixed), fixed amount where used | Computed PhilHealth deduction line       |
| **HDMF**                      | Contribution Calculation, Schedule, Rules | Entitled to HDMF, mode (fixed, % of base pay, or mixed)                | Computed HDMF line                       |
| **HDMF Voluntary / Modified** | Contribution Calculation, Schedule        | Entitled to HDMF Voluntary or Modified, employee-level amount          | Separate voluntary or modified HDMF line |

#### What should administrators know about SSS contribution timing?

If the company deducts SSS **every payroll**, Ashima does not always split the amount evenly. For semi-monthly payroll, Ashima may split or rebalance the monthly amount. For the second payroll of the month, Ashima checks what was already deducted in the first payroll so the employee does not exceed the required monthly total

#### What does Contribution Calculation control?

This page controls which contribution methods the company allows for:

* **SSS**
* **PHIC**
* **HDMF**

Examples from the rule set include:

* **SSS Contribution Table**
* **SSS Fixed Rate**
* **PhilHealth Contribution Table**
* **PhilHealth Fixed Rate**
* **HDMF Fixed 100**
* **HDMF % of Base Pay**
* **HDMF Mixed Deduction**
* **HDMF Voluntary Increase**
* **HDMF Modified**

These are company-level options. They do not deduct money by themselves until the employee is entitled and assigned to the matching contribution mode.

#### What does Contribution Schedule control?

This page controls when each contribution is deducted in the payroll month.

Available schedule patterns include:

* **first payroll of the month**
* **second payroll of the month**
* **last payroll of the month** when the company has fortnightly payroll
* **every payroll**

This is important because the same employee entitlement can produce different payroll timing depending on the company contribution schedule.

#### What do Contribution Rules control?

This page controls which pay items count when payroll computes contributions.

In practice, this can include:

* basic pay
* selected earning families such as **Allowance**, **Other Earnings**, or **De Minimis**, if the company includes them
* selected payroll adjustments that the company wants included in contribution basis

So contribution amounts are not always based on base pay alone. They can change depending on which earnings and payroll corrections the company includes in the rule.

#### What does the employee-level contribution profile control?

The employee compensation page is where the admin applies the contribution profile to the employee.

At employee level, the admin can control:

* whether the employee is entitled to **SSS**
* whether the employee is entitled to **PhilHealth**
* whether the employee is entitled to **HDMF**
* whether the employee is entitled to **HDMF Voluntary**
* whether the employee is entitled to **HDMF Modified**
* which method applies to the employee when more than one company method is allowed
* fixed contribution amounts when the employee uses a fixed mode
* employee-share percentage in mixed HDMF setup
* voluntary and modified HDMF amounts where enabled

#### How do the main contribution types work?

| Contribution type                  | Company settings that drive it                                      | Employee-level controls                                                                 | What payroll shows later                                                     |
| ---------------------------------- | ------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------- |
| **SSS**                            | Contribution Calculation, Contribution Schedule, Contribution Rules | Entitled to SSS, SSS mode such as table or fixed, fixed amount where used               | Computed **SSS** deduction line in payroll and payslip                       |
| **PHIC**                           | Contribution Calculation, Contribution Schedule, Contribution Rules | Entitled to PhilHealth, PhilHealth mode such as table or fixed, fixed amount where used | Computed **PhilHealth** deduction line in payroll and payslip                |
| **HDMF I**                         | Contribution Calculation, Contribution Schedule, Contribution Rules | Entitled to HDMF, HDMF mode such as fixed, % of base pay, or mixed deduction            | Computed **HDMF** line in payroll and payslip                                |
| **HDMF II / Modified / Voluntary** | Contribution Calculation, Contribution Schedule                     | Entitled to HDMF Voluntary or Modified HDMF, employee-level amount where enabled        | Separate voluntary or modified HDMF line in payroll and payslip when enabled |

#### What should administrators know about employee contribution modes?

#### How are contributions shown in payroll review?

In payroll review, contributions do not appear like reusable assigned deduction rows.

Instead, they appear as computed payroll lines such as:

* **SSS**
* **PhilHealth**
* **HDMF**
* **HDMF I**
* **HDMF II**
* voluntary contribution lines where enabled

These are payroll outputs, not simple manually assigned deduction-type rows.

#### How are contributions shown in masterlist and reports?

On the masterlist page itself, contributions are included in payroll totals rather than displayed as reusable per-type deduction cards.

In reports and downloads, contributions are treated as standard payroll columns, such as:

* employee **SSS**
* employee **PhilHealth**
* employee **HDMF**
* voluntary contribution amounts where applicable

So contributions are easier to review as payroll result columns than as reusable type listings.

#### How are contributions shown on the payslip?

The payslip shows contributions as their own top-level deduction lines.

Depending on the employee’s setup and the company rules, the payslip can show:

* **SSS**
* **PhilHealth**
* **HDMF**
* **HDMF I**
* **HDMF II**
* voluntary or modified HDMF lines

This is one of the clearest signs that contributions are treated as computed payroll outputs rather than reusable assigned deduction records.

#### What should administrators know about contribution settings?

An employee can be entitled to a contribution but still follow different allowed methods.

Examples:

* **SSS** can follow the table or a fixed amount
* **PhilHealth** can follow the table or a fixed amount
* **HDMF** can follow fixed 100, percent of base pay, or mixed deduction

So when contribution results look different between employees, check both entitlement and the selected employee method.

Contribution timing and schedule can be set at company level as a default, then overridden at employee level when a specific employee needs different contribution handling.

#### What should administrators know about SSS timing?

SSS timing can vary based on the employee contribution payment setting.

Common timing options include:

* first payroll of the month
* second payroll of the month
* every payroll
* last payroll of the month for some payroll schedules

When SSS is set to **every payroll**, the system can either:

* split the monthly SSS contribution across payrolls, or
* compute the remaining amount needed later in the month based on accumulated payroll amounts

This is why the SSS deduction in the second payroll of the month may differ from the first payroll.

#### How does SSS calculation work?

SSS depends on two things:

1. the company setting for how SSS is calculated
2. the employee setting for which SSS method applies

The common methods are:

* **SSS Contribution Table**
* **SSS Fixed Rate**

#### What is the simple formula for SSS when the employee uses the SSS table?

Ashima first builds the employee's SSS contribution basis from the employee's monthly-equivalent basic pay.

It then adds or subtracts the pay items the company includes in **Contribution Rules**.

That basis can include:

* basic pay
* selected earnings
* selected payroll adjustments
* and, if the company chooses, it can reduce the basis by absences, tardiness, or undertime

Then Ashima matches that basis to the SSS table range and takes the employee share for that range.

Use this guide:

`SSS Basis = Monthly-equivalent basic pay + included earnings and adjustments - included deduction-side reductions`

`SSS Employee Share = Table amount for the matching SSS basis range`

#### What is the simple formula for SSS when the employee uses a fixed rate?

Use this guide:

`SSS = Fixed SSS amount assigned to the employee`

#### How does SSS behave when the company deducts SSS every payroll?

If the company deducts SSS **every payroll**, Ashima does not always split the amount evenly.

Common behavior:

* **Semi-monthly**: Ashima may split or rebalance the monthly amount across the payrolls in the month
* **Weekly**: the amount can be split across the weekly payrolls
* **Second payroll of the month**: Ashima checks what was already deducted in the first payroll so the employee does not go over the required total
* **fixed and table-based setups** can behave differently

**Example**

* Monthly SSS employee share from the table: `1,000`
* First semi-monthly payroll deduction: `500`
* Second semi-monthly payroll deduction: `500`

Total SSS for the month stays within the required monthly amount for that employee's setup.

#### What other formulas should this guide include later?

The next useful payroll formulas to add are:

* **Taxable Pay**
* **Gross Pay**
* **Withholding Tax basis**
* **PhilHealth**
* **HDMF**
* **Leave monetization**
* **Open Shift required-hours effect on payroll**

These are worth documenting because they change payroll results and are often reviewed during payroll disputes.

#### How does SSS calculation work?

SSS depends on the company contribution method setting and the employee contribution mode.

**Table-based SSS:**

```
SSS Basis = Monthly-equivalent basic pay + included earnings and adjustments - included deduction-side reductions

SSS Employee Share = Table amount for the matching SSS basis range
```

**Fixed SSS:**

```
SSS = Fixed SSS amount assigned to the employee
```

#### What payroll formulas should be added in the next update?

* Taxable Pay detailed build
* Gross Pay detailed build
* Withholding Tax basis
* PhilHealth
* HDMF
* Leave monetization
* Open Shift required-hours effect on payroll
