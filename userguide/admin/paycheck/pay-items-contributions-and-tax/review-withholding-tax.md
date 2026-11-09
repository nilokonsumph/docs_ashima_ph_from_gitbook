# review withholding tax

## review withholding tax

This means the final withholding-tax amount in payroll is shaped by:

* the company computation basis
* the company schedule and method
* the employee’s tax status
* the employee’s actual taxable payroll result

### what company settings control withholding tax?

Ashima splits the company-side tax setup into two main pages:

* **Withholding Tax Rule** — which compensation basis the company uses for tax computation
* **Withholding Tax** — the schedule and method assigned by rank

### what does Withholding Tax Rule control?

This page controls the company tax computation basis.

In simple terms, it answers:

* what compensation base the company uses when computing withholding tax

The setup loads a company default and can be updated from the withholding-tax rule page. This is a company-level tax rule, not an employee-assigned tax item.

### what does the Withholding Tax schedule page control?

This page controls the company’s withholding-tax deduction schedule by rank.

The settings include:

* **rank**
* **description**
* **schedule**
* **withholding tax method**

So the company can define how tax timing and tax method apply to different ranks instead of using one flat rule for everyone.

### what does the employee tax profile control?

The employee compensation page carries the employee tax profile that payroll uses when computing withholding tax.

This includes:

* the employee’s **tax status**
* whether the employee follows the normal payroll tax path or a fixed-tax setup where used
* the employee record that payroll reads together with taxable pay for the run

If withholding tax looks wrong, check the employee tax profile first before changing payroll entries.

### what is the difference between Withholding Tax, Withholding Tax (Adjustments), and Withholding Tax (Fixed)?

* **Withholding Tax** — the normal payroll-calculated tax result
* **Withholding Tax (Adjustments)** — a payroll tax correction for the current run
* **Withholding Tax (Fixed)** — a fixed tax amount used when that tax method applies to the employee

### how is withholding tax shown in payroll review?

In payroll review, admins can encounter three separate tax lines:

* **Withholding Tax (Adjustments)**
* **Withholding Tax**
* **Withholding Tax (Fixed)**

The employee pay details page also shows a withholding-tax computation breakdown, so admins can review how the final tax amount was reached.

### how is withholding tax shown on the masterlist and in reports?

On the masterlist page itself, withholding tax is shown as part of the employee payroll summary under the **Total Withholding Tax** column.

In reports and exports, withholding tax is treated as a standard payroll output column rather than a reusable deduction type.

So it is reviewed as a payroll result, not as a company deduction type assigned one employee at a time.

### how is withholding tax shown on the payslip?

The payslip shows withholding tax as top-level tax lines.

Depending on what applies to the employee and payroll run, the payslip can show:

* **withholding tax**
* **Withholding Tax (Fixed)**

Tax adjustments can also appear in the pay details flow as their own tax-adjustment amount before the final payslip breakdown is reviewed.

### what should administrators know about withholding-tax adjustments?

Withholding-tax adjustments are not the same as changing the employee’s tax status or the company tax rule.

Use them when a payroll-side tax correction is needed for the current run.

They affect the payroll output for that run, but they do not replace:

* the company withholding-tax rule
* the company withholding-tax schedule
* the employee’s normal tax status profile

### what should administrators know about Withholding Tax?

Withholding tax is a payroll-calculated result, not a reusable deduction row.

Payroll computes it from:

* the company withholding-tax rule
* the company withholding-tax schedule and method
* the employee’s tax profile
* the employee’s taxable payroll result for that run

Separate tax adjustments or fixed-tax entries can still change the final number for a specific payroll run.

### how does withholding tax move from setup to payroll output?

Withholding tax follows a three-layer workflow:

1. set the company withholding-tax computation rule
2. set the withholding-tax deduction schedule by rank
3. maintain the employee’s tax status in the employee compensation profile

This means the final withholding-tax amount in payroll is shaped by:

* the company computation basis
* the company schedule and method
* the employee’s tax status
* the employee’s actual taxable payroll result
