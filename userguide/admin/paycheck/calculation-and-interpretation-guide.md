# calculation and interpretation guide

## calculation and interpretation guide

### what is the difference between monthly-paid and daily-paid employees?

**pay rate type** determines how basic pay is built. **pay schedule** determines how often payroll is processed. a daily-paid employee can belong to a semi-monthly pay schedule; that does not turn the employee into a monthly-paid employee.

| pay rate type                   | basic-pay starting point                                                              | example before other payroll items        |
| ------------------------------- | ------------------------------------------------------------------------------------- | ----------------------------------------- |
| **By Month**, paid semi-monthly | monthly salary ÷ 2 for a full period without proration or a salary change             | ₱30,000 ÷ 2 = ₱15,000                     |
| **By Month**, paid monthly      | full monthly salary for a full period without proration or a salary change            | ₱30,000 monthly salary = ₱30,000          |
| **By Day**                      | total of eligible paid workdays multiplied by the daily rate applicable to each date  | 10 eligible days × ₱700 = ₱7,000          |
| **By Hour**                     | total of payable regular hours multiplied by the regular rate applicable to each date | 80 payable regular hours × ₱150 = ₱12,000 |

these are basic-pay starting amounts, not take-home pay. review attendance deductions, premiums, earnings, contributions, tax and other deductions separately. a monthly salary's derived daily reference rate is also different from an employee being paid **By Day**: see [Pay Rate Calculation settings](run-payroll/configure-paycheck-before-running-payroll.md#how-does-pay-rate-calculation-affect-payroll).

### payroll calculation examples

#### how is payroll calculated in Ashima?

use these formulas to explain how Ashima builds pay. The examples below are simplified so administrators can understand the result they see in payroll review.

#### what is the general net pay formula in Ashima?

Ashima builds payroll in this order:

1. **Regular earnings base**
2. **Taxable pay**
3. **Non-taxable pay**
4. **Gross pay**
5. **Net pay**

use this simple reconciliation pattern:

> **Gross Pay = Taxable Pay + Non-Taxable Pay**

> **Net Pay = Gross Pay - Total Deductions**

**Total Deductions** is the combined deduction amount used by that payroll result. depending on the output, withholding tax, contributions, loans and other deductions may also appear as separate detail columns or rows. do not subtract a separately displayed component again when it is already included in **Total Deductions**.

**how is net pay calculated for monthly-paid employees?**

**for a monthly-paid employee,** the starting point is the employee's cutoff basic pay.

use this simple guide:

> **Regular Earnings Base = Basic Pay - Absences - Tardiness - Undertime**

> **Taxable Pay = Regular Earnings Base + taxable earnings and taxable payroll adjustments**

> **Non-Taxable Pay = non-taxable earnings**

> **Net Pay = Taxable Pay + Non-Taxable Pay - total deductions**

**for a semi-monthly monthly-paid employee**, the basic pay usually starts from:

> **Basic Pay = Monthly Rate / 2**

for monthly payrolls, Ashima uses the full monthly rate. if the employee joins mid-period or has a mid-period salary increase, Ashima can replace the flat starting amount with a prorated amount for the covered cutoff.

**Example**

* Monthly rate: `30,000`
* Semi-monthly basic pay: `15,000`
* Absences: `1,000`
* Tardiness: `200`
* Taxable allowance: `500`
* Withholding tax and deductions combined: `2,300`

`Regular Earnings Base = 15,000 - 1,000 - 200 = 13,800`

`Taxable Pay = 13,800 + 500 = 14,300`

`Net Pay = 14,300 - 2,300 = 12,000`

***

**how is net pay calculated for hourly-paid employees?**

For hourly-paid employees, Ashima starts from payable rendered hours.

Use this simple guide:

> **Basic Pay = Payable Hours x Hourly Rate**

> **Regular Basic Pay = sum of payable regular hours x the applicable regular rate for each date or rate segment**

> **Net Pay = Taxable Pay + Non-Taxable Pay - total deductions**

**Example**

* Payable hours: `80`
* Hourly rate: `150`
* Basic pay: `12,000`
* Overtime pay: `600`
* Total deductions after tax and contributions: `1,900`

`Taxable Pay = 12,000 + 600 = 12,600`

`Net Pay = 12,600 - 1,900 = 10,700`

this example assumes the 80 hours are already payable regular hours. if the detailed result shows a separate tardiness or undertime deduction, reconcile it once; do not reduce payable hours and subtract the same shortfall again.

**how is net pay calculated for daily-paid employees?**

For daily-paid employees, Ashima starts from payable rendered days.

Use this simple guide:

> **Basic Pay = sum of eligible paid workdays x the applicable fixed daily rate for each date or rate segment**

> **Taxable Pay = Basic Pay + taxable additions and premiums**

> **Net Pay = Taxable Pay + Non-Taxable Pay - total deductions**

**Example**

* Payable days: `10`
* Daily rate: `700`
* Basic pay: `7,000`
* Holiday pay: `500`
* Total deductions after tax and contributions: `1,000`

`Taxable Pay = 7,000 + 500 = 7,500`

`Net Pay = 7,500 - 1,000 = 6,500`

this example assumes ten eligible paid workdays. when an absence is already excluded from the eligible-day count, do not subtract that same day again. use the saved date-level breakdown and deduction rows to determine how the actual result was built.

***

#### how is salary calculated for a new employee who joins mid-period?

Ashima can prorate a mid-period joiner instead of using the full cutoff amount. the selected calculation branch depends on the employee's pay type, pay schedule and company proration settings.

use this guide:

* **Monthly-paid**: rendered payroll amounts from hire date to cutoff end, based on the employee's schedule and payable time
* **Hourly-paid**: payable hours from hire date onward x hourly rate
* **Daily-paid**: payable days from hire date onward x daily rate

when the new-hire actual method applies to a semi-monthly monthly-paid employee, use:

> **Prorated Basic Pay = (Starting Monthly Salary / 2) x Employed Workdays / Cutoff Workdays**

**Example: monthly-paid new hire**

* Monthly rate: `30,000`
* Employed workdays in the cutoff: `6`
* Total cutoff workdays: `12`

`Prorated Basic Pay = (30,000 / 2) x 6 / 12 = 7,500`

this actual-method example is not a universal thirty-day or twenty-six-day divisor. another configured proration or salary-change rule can select a different calculation.

***

For a salary change that takes effect inside a pay period, see [review salary increase details](salary-increases-and-retroactive-pay/review-salary-increase-details.md#page-98). That article owns the applicable formulas, pay-type differences, DIH treatment, examples, and verification steps.

***

### how do pay rate type and pay schedule change basic pay?

**pay rate type** describes the unit of the employee's salary: By Month, By Day or By Hour. **pay schedule** describes how often payroll is processed, such as Semi Monthly or Monthly. check both before comparing two employees. a group name alone does not prove the employee's pay rate type.

for a full-period employee with no salary change or proration, By Month with Semi Monthly starts from monthly basic salary ÷ 2; By Month with Monthly starts from the monthly basic salary. daily and hourly payroll instead build basic pay from eligible date-level amounts. deductions, premiums, allowances and tax must then be reconciled separately.

#### can you show a monthly-paid example?

assume a monthly basic salary of ₱30,000, a Semi Monthly schedule, full-period employment, no salary change, and no proration. basic pay before deductions is ₱30,000 ÷ 2 = **₱15,000**. this is the basic-pay starting amount, not take-home pay.

#### why is daily-paid payroll different?

daily payroll uses the applicable daily rate for each eligible paid workday. for ten eligible workdays at ₱700, the illustrative basic-pay total is 10 × ₱700 = **₱7,000**. if five eligible days use ₱700 and five use ₱750 following an effective salary increase, the total is (5 × ₱700) + (5 × ₱750) = **₱7,250**.

do not reduce a fixed daily rate in proportion to short logged hours and then deduct the same shortfall again. the daily-rate breakdown distinguishes the basic-pay amount from separate attendance deductions. use the actual eligible dates and saved deductions when reconciling the run.

#### what should I check for hourly-paid payroll?

check the payable hours and applicable rate for each date, including any salary-change date. as an arithmetic illustration, 40 payable hours at ₱150 plus 40 at ₱160 totals **₱12,400** before other pay items and deductions. this example assumes those hours have already been established as payable; it does not mean that every clocked hour is paid, or that overtime is paid at the regular hourly rate. check the hours breakdown, schedule and applicable premiums first.

#### how can a new hire's monthly basic pay be prorated?

when the new-hire actual method applies to Semi Monthly payroll, use:

**(starting monthly salary ÷ 2) × employed workdays ÷ cutoff workdays**.

for ₱30,000 monthly salary, six employed workdays and twelve cutoff workdays, this gives (₱30,000 ÷ 2) × 6 ÷ 12 = **₱7,500**. use the method and workday counts applicable to that employee; this is not a universal thirty-day or twenty-six-day divisor. salary-change and other proration settings can select a different calculation branch.

#### how do I avoid deducting withholding tax twice?

reconcile the headings in the output you are using. a separate displayed tax column does not necessarily mean tax must be subtracted again after Total Deductions. for example, **₱90,758.80 gross − ₱18,037.52 Total Deductions = ₱72,721.28 Net Pay**. if the output also shows withholding tax of ₱17,417.41 separately, do not subtract it again. use this check to reconcile displayed totals; it does not calculate the tax rate.
