---
description: >-
  use salary increase details to understand how a saved, effective-dated salary
  change affected an employee's regular pay in the current payroll period.
---

# salary increase details

{% hint style="info" %}
a change to compensation that affects an open pay run requires payroll recalculation before you rely on the result.
{% endhint %}

**navigation:**\
go to **paycheck → pay run → employee pay details**.

### when does salary increase detail appear?

salary increase detail appears when the employee has a salary increase whose effective date falls inside the payroll period. an information action beside basic pay opens the calculation when the breakdown is available.

the detail separates:

* salary before the increase
* salary after the increase
* effective date
* workdays or time covered by each rate
* each increase when more than one increase falls inside the period
* absence, tardiness, and undertime deductions when applicable
* final regular pay

if the salary change has not yet been entered, start with increase one employee's salary or update salaries in bulk.

### how is a monthly salary increase calculated?

for a semi-monthly payroll, the calculation starts with the employee's old half-month salary. the system then adds only the portion of each increase that applies from its effective date to the end of the cutoff.

```
old salary component = old monthly salary / 2

increase component =
(new monthly salary - old monthly salary) / 2
x applicable workdays from effective date
/ total cutoff workdays

regular pay before dih = old salary component + all increase components

final regular pay = regular pay before dih - dih deductions
```

dih means deductions for absences, tardiness, and undertime. for a monthly payroll, the calculation uses the full monthly period instead of dividing the salary by two.

### what happens when there is more than one increase?

the detail shows each increase separately. each component uses its own effective date and the number of applicable workdays remaining in the cutoff.

```
regular pay before DIH =
original salary component
+ first increase component
+ second increase component
+ any later increase components
```

use the increase tabs to trace each effective date, previous salary, updated salary, and prorated component.

### how is a daily-paid employee calculated?

the system applies the daily rate effective on each eligible paid date.

```
regular pay = sum of eligible paid days x daily rate applicable on each date
```

dates before the increase use the old daily rate. the effective date and later eligible dates use the updated daily rate.

### how is an hourly-paid employee calculated?

the system applies the hourly rate effective on each eligible paid hour.

```
regular pay = sum of eligible paid hours x hourly rate applicable on each date
```

review the dated regular-hours entries to see which rate applies before and after the effective date.

### how are regular shifts and open shifts different?

for a regular-shift employee, the system uses the assigned schedule to determine expected workdays and hours.

for an open-shift employee, the system uses recognized open-shift time and the applicable rate. the detail identifies undertime when the recognized hours are below the required hours. it does not treat an open-shift employee as having the same fixed daily schedule as a regular-shift employee.

review the rate, divisor, eligible hours, and effective-date split shown in the calculation before finalizing payroll.

### what happens after payroll recalculation?

the employee pay details and payslip use the recalculated regular pay. the payslip remains the official payroll result, while salary increase details explain how that result was produced.

### why does a past effective date not appear here?

an increase that belongs to a payroll period already processed requires retroactive pay. use the retroactive-pay process to calculate the unpaid difference across those earlier periods.

### related articles

* salary increase
* increase one employee's salary
* update salaries in bulk
* retroactive pay
