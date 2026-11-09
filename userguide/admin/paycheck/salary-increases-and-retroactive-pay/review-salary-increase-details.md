# review salary increase details

## review salary increase details

{% hint style="info" %}
a compensation change that affects an open pay run requires recalculation before the payroll result can be relied on.
{% endhint %}

**Navigation:** Go to **Paycheck → Pay Run → Employee Pay Details**. Open the information action beside **Basic Pay** when salary-increase details are available.

### what does salary increase detail explain?

the detail explains how regular pay was built when a new basic-pay rate became effective inside the payroll period. it separates the rate before the increase, the rate from the effective date onward, applicable workdays or payable time, DIH deductions, and final regular pay. salary increase changes **Basic Pay**; it is not a separate earning added on top.

DIH means absence, tardiness, and undertime deductions. these deductions are applied using the rate applicable when the deficiency occurred.

### which date determines the calculation?

the effective date is inclusive. eligible work or payable time before that date uses the previous rate. eligible work or payable time on and after that date uses the new rate.

if the effective date is the first applicable day of the period, the new rate can apply to the full period and a split may not be needed. if it falls on a rest day or another non-payable date, that date contributes no payable workday by itself; the new rate applies to the next eligible time on or after the effective date.

### what is the formula for a semi-monthly, monthly-paid employee?

for the validated semi-monthly calculation, Ashima starts with the previous half-month salary and prorates only the increase from the effective date through the cutoff end.

```
previous salary component = previous monthly salary / 2

increase component =
(new monthly salary - previous monthly salary) / 2
x applicable workdays from effective date
/ total cutoff workdays

salary-adjusted basic pay before DIH =
previous salary component + all applicable increase components

final regular pay =
salary-adjusted basic pay before DIH - DIH deductions
```

for a monthly payroll, use the full-period salary basis instead of the semi-monthly division by two. use the workday counts and rates displayed by Ashima for the employee rather than substituting calendar days.

### worked example: mid-period monthly salary increase

assume the following values:

* previous monthly salary: `45,000`
* new monthly salary: `50,000`
* total cutoff workdays: `11`
* applicable workdays from the effective date: `2`

```
previous salary component = 45,000 / 2 = 22,500.00

increase component =
(50,000 - 45,000) / 2 x 2 / 11
= 454.55

salary-adjusted basic pay before DIH =
22,500.00 + 454.55
= 22,954.55
```

if the detail shows DIH deductions of `1,061.40`, then:

```
final regular pay = 22,954.55 - 1,061.40 = 21,893.15
```

### how are DIH deductions split before and after the increase?

Ashima prices a deficiency using the rate in effect on its date. for a semi-monthly monthly-paid employee, the displayed hourly-rate basis can be expressed as:

```
hourly rate =
monthly salary / 2 / cutoff workdays / average working hours per day
```

therefore:

```
DIH deduction =
(deficiency hours before the effective date x previous hourly rate)
+ (deficiency hours on or after the effective date x new hourly rate)
```

**Average Working Hours Per Day** comes from the applicable payroll-calendar setting. it is a rate divisor and is not necessarily the same as the hours visibly worked by an open-shift employee.

### how is paid leave treated for monthly-paid employees?

paid leave can remain visible in the earnings breakdown, but it is already covered by monthly basic pay. do not add the paid-leave row a second time when reconciling salary-adjusted basic pay. unpaid leave and other DIH effects must be reviewed according to the displayed deduction breakdown.

### how is a daily-paid employee calculated?

Ashima applies the daily rate effective on each eligible paid date.

```
regular pay =
sum of eligible paid days x daily rate applicable to each date
```

dates before the effective date use the previous daily rate. the effective date and later eligible dates use the new daily rate. when hours are needed for a partial-day deduction, the daily rate is converted using the applicable average working hours per day.

### how is an hourly-paid employee calculated?

Ashima prices each eligible regular-hour row using the rate effective on that date.

```
regular pay =
(hours before effective date x previous hourly rate)
+ (hours on or after effective date x new hourly rate)
```

the effective date belongs to the new-rate portion. displayed hours can be rounded, so reconcile the saved row amounts when a manual multiplication differs by a small rounding amount.

### how does open shift affect the explanation?

a monthly-paid open-shift employee can still use the monthly salary-difference proration shown above. the open-shift hours displayed in payroll follow the period's recognized hours and open-shift cutoff. the hourly-rate explanation uses **Average Working Hours Per Day** as a divisor. do not treat that divisor as the employee's daily open-shift cap.

### what happens when more than one increase affects the period?

Ashima can save another salary change for an employee whose compensation history already contains a change in the same pay period. The manual Salary Increase form displays a conflict warning and states that proceeding creates another retroactive-pay entry. The bulk salary-update import is stricter and rejects a row when another active salary increase already falls within the same pay-period coverage.

For an open pay period, each saved rate must apply only from its own effective date. For example, if a first increase takes effect on the 5th and a second takes effect on the 20th, the expected sequence is the previous rate before the 5th, the first new rate from the 5th through the 19th, and the second new rate from the 20th onward.

{% hint style="warning" %}
Do not assume that saving a second increase automatically proves that the open-payroll detail preserved both segments. Recalculate the pay run and confirm that every saved effective date, rate, workday or hour range, and component amount appears. If the detail shows only the latest change or the dates overlap unexpectedly, stop and reconcile compensation history before approving payroll.
{% endhint %}

For a closed period, the additional salary change can create another Retroactive Pay record. Review the repeated and overlapping-retro guidance in the Retroactive Pay article before accepting the new result.

### what should I verify after recalculation?

check all of the following:

1. previous and new basic pay;
2. effective date and covered payroll period;
3. employee pay-rate type and pay schedule;
4. total and applicable workdays, days, or hours;
5. **Average Working Hours Per Day** when an hourly equivalent is shown;
6. DIH rows before and after the effective date;
7. paid-leave treatment;
8. salary-adjusted basic pay, final regular pay, and the resulting payslip.

for an effective date in a payroll period already processed, use the Retroactive Pay article.

### related articles

* increase an employee's salary
* update salaries in bulk
* recalculate and review retroactive pay
* calculation and interpretation guide
