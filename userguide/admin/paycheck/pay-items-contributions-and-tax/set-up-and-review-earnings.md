# set up and review earnings

## set up and review earnings

Use the Earnings area to review employee compensation setup, assign earning entries to employees, and check which items will flow into payroll and payslip output.

**Navigation:** Go to **Paycheck → Earnings**

### what is the normal earnings workflow?

For most earnings, the workflow has two layers:

1. create the earning type in **Settings**
2. assign or generate the earning at employee level
3. include the employee in a payroll run.
4. the earning appears in payroll review, masterlist totals, and the payslip.

This matters because the company setup defines the earning rule, while the employee record defines who gets it and how much is applied.

### what is set globally and what can still be set per employee?

Some earnings are fully reusable earning types. Others are only enabled globally and then produced through a separate payroll flow.

* **Global setup** defines the earning name, schedule logic, tax rule, and other default payroll behavior.
* **Employee assignment** applies the earning to a specific employee and usually sets the actual amount or active status.
* some fields stay locked to the earning type
* some fields can still be changed per employee

### how should administrators understand taxable and non-taxable earnings?

* **Taxable** earnings increase taxable pay and can affect withholding tax.
* **Non-taxable** earnings still increase pay, but they stay on the non-taxable side unless a limit or excess rule says otherwise.
* some earnings, such as **De Minimis**, stay non-taxable only up to the allowed ceiling

### how do earnings move from setup to payroll output?

Most earning groups start with a company-level type created in **Settings**, followed by employee-level assignment, and then appear in payroll review, masterlist, and payslip output.

| Earning type        | Setup pattern                                                 | Global setup page                                                             | What the global setup controls                                                                                         | What the employee-level record controls                                                                                          | How it appears in admin payroll review                                                                  | How it appears in masterlist or download                                                                                            | How it appears on the payslip                                                                            |
| ------------------- | ------------------------------------------------------------- | ----------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **Allowance**       | Reusable earning type, then assigned to employees             | **Settings → Paycheck → Earnings → Allowance**                                | Name, tax rule, pay schedule, frequency, variability type, amount logic, absent entitlement, applicable employee group | Assigned employee, actual amount or rate value, employee-level status, employee-level absent entitlement                         | Reviewed as its own **Allowances** earning block, then folded into payroll totals                       | Masterlist page: inside totals only. Masterlist download: allowance family can be selected and broken out into its own columns      | Shows as its own **Allowance** earning group; payroll-entry versions can also appear under **Ingestion** |
| **De Minimis**      | Global rule plus employee-level eligibility and rows          | **Settings → Paycheck → Earnings → Deminimis**                                | De minimis type, rate type, tax-exempt ceiling, excess rule, payroll schedule, destination, start rule                 | Employee entitlement, assigned amount or rate value, credits, schedule details, effective start                                  | Reviewed as its own **De Minimis** earning block; excess is reviewed separately when applicable         | Masterlist page: inside totals only. Masterlist download: de minimis family can be selected and broken out into its own columns     | Shows in the de minimis earnings area; any excess is shown separately based on the rule                  |
| **Other Earnings**  | Reusable earning type, then assigned or released to employees | **Settings → Paycheck → Earnings → Other Earnings**                           | Name, description, recurring rule, pay date or schedule, default amount, tax rule                                      | Employee amount, active record, occurrence or interval details, release timing, employee-level tax setting carried from the type | Reviewed as its own **Other Earnings** block; paycheck-entry versions appear as earnings-side ingestion | Masterlist page: inside totals only. Masterlist download: other-earnings family can be selected and broken out into its own columns | Shows as earnings; paycheck-entry versions usually appear under **Ingestion**                            |
| **13th Month**      | Separate payroll process, not a reusable monthly earning type | **Settings → Paycheck → Earnings → 13th Month** and related entitlement rules | Company 13th-month rules and what the process includes                                                                 | Employee entitlement, inclusion in the run, employee-specific run result                                                         | Handled in the dedicated 13th month flow, not in the normal payroll earning blocks                      | Reported in the dedicated 13th-month and year-end outputs, not as a reusable earning column in the regular payroll masterlist       | Shown on the dedicated 13th month payslip                                                                |
| **Retroactive Pay** | Feature enablement plus employee-level generated records      | **Settings → Paycheck → Earnings → Retroactive Pay**                          | Feature on or off only                                                                                                 | Retro result from compensation history, effective date, covered period, rates, hours, generated retro amount                     | Reviewed as its own **Retroactive Pay** block after retro is generated                                  | Reflected in payroll totals and retro outputs; not treated like a reusable allowance-style column                                   | Shown as a separate retroactive-pay line when generated                                                  |

### how are these earnings handled in payroll?

Not all earnings are managed the same way in Ashima.

**Allowance** and **Other Earnings** are first created in Settings, then assigned to employees. Use these when you want to create an earning type once and reuse it across employees.

\
**De Minimis** starts from a company rule in Settings, then you apply it to employees who are entitled to it. Use this when the company wants one shared rule, but employees can still have their own assigned amount or eligibility.

\
**13th Month** is not assigned like a regular earning. It is handled through the separate 13th Month payroll process. Use this when you are preparing the company's 13th month run.

{% hint style="info" %}
The easiest way to remember it is:\
\
Allowance / Other Earnings = create, then assign\
De Minimis = set the company rule, then apply to eligible employees\
13th Month = run through the 13th month process<br>
{% endhint %}

### what fields are usually inherited from the earning setup?

For reusable earning types, the employee assignment does not start from scratch. It usually inherits the earning’s configured values:

* earning name or type
* tax rule
* schedule or frequency rule
* variability rule
* cap, ceiling, or excess rule where applicable

### what fields are usually set or changed at employee level?

The employee-side record usually controls:

* who receives the earning
* the assigned amount
* whether the employee record stays active, paused, or completed
* employee-specific schedule details when the earning supports them

For some earnings, the employee-level page can also override practical details such as:

* whether the employee remains entitled while absent
* the flat amount or percentage-based value

### what should administrators expect when assigning an allowance?

Allowance is one of the clearest examples of global setup plus employee-level override.

The global allowance type can define:

* allowance name
* frequency
* variability type
* pay schedule
* tax rule
* whether the allowance remains payable even when the employee is absent
* which employee groups the allowance applies to

At employee level, the admin can still work with:

* the selected allowance type
* the employee amount for flat-rate allowances
* the daily-rate or hourly-rate percentage for variable allowances
* pay status such as active, paused, or completed
* the employee-level absent entitlement flag

In payroll review:

* the allowance does not become its own visible masterlist table column on the page
* it is included in payroll totals on the masterlist page
* it can still be broken out in downloads and appears as its own allowance group in payslip review

### what should administrators expect when assigning De Minimis?

De minimis also starts in **Settings**, but its rule set is more payroll-driven.

The global setup can define:

* de minimis type
* rate type
* frequency
* payroll schedule
* destination
* tax-exempt status
* de minimis ceiling
* start rule and proration behavior

At employee level, the admin can then apply:

* the employee amount or rate-based value
* the effective start details
* the assigned destination or release pattern

The important payroll rule is that de minimis can stay non-taxable only up to the configured ceiling. Excess can move into taxable treatment based on the configured rule.

This is why de minimis behaves less like a simple reusable allowance and more like a company rule that is then applied to the employee.

### what should administrators expect when assigning Other Earnings?

Other Earnings are reusable earning types created in **Settings**, then assigned or released for employees.

The global setup can define:

* earning name
* description
* amount
* whether the earning is recurring
* whether it is taxable or non-taxable
* payroll schedule, pay date, interval, or occurrence rule

At employee or payroll level, the admin then controls:

* which employee receives the earning
* the amount to be applied
* the timing of release

The key rule here is the tax setting:

* **Taxable Other Earnings** increase taxable pay
* **Non-taxable Other Earnings** increase pay without going through taxable-pay treatment in the same way

In payroll review:

* other earnings are included in payroll totals on the masterlist page
* selected downloads can break them out by earning type
* payslip output can show them as their own earnings rows or as earnings-side ingestion entries, depending on how they were added

When you add **Other Earnings** from the paycheck adjustment page, payroll uses the taxable paycheck-entry version. Use the regular employee earning assignment flow when you need the non-taxable setup version.
