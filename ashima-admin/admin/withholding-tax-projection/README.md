# Withholding tax projection

use the withholding tax projection tool to estimate an employee's year-end taxable income and spread a recommended withholding adjustment across remaining pay periods.

**Navigation:**\
go to **Reports → Tax → Wtt Tool**.

### what should be ready before you use the tool?

Review the selected year, payroll calendars, employee payroll-group assignment, current payroll and tax values, employee tax information, 13th-month assumption, and any saved plus adjustment.

The projection is only as reliable as those source records. Correct employee, payroll, or calendar information at its source, then recalculate the projection.

### what does the tool use?

the projection starts from the employee's current year values, payroll-group calendar, projected 13th month, annual withholding-tax table, and any saved plus adjustment.

the current released calculation uses scheduled lapsed and remaining pay periods. It does not use the unreleased T-0020 proposal for actual closed-payslip counting.

### what is the simple formula?

```
projected net taxable
= current net taxable
+ taxable projected 13th month
+ projected future net taxable

recommended adjustment per pay
= (projected tax due - current tax withheld + plus adjustment)
  / remaining pay periods
```

when one or no future period remains, the tax gap is not divided across multiple periods.

### how is the 13th month treated?

the projected 13th-month amount first uses the employee's remaining space under the non-taxable 90,000 limit. Only the excess becomes taxable in projected net taxable.

### how is future taxable income estimated?

```
average taxable per lapsed period
= current net taxable / lapsed scheduled pay periods

projected future net taxable
= average taxable per lapsed period x remaining scheduled pay periods
```

the result is an estimate. Recalculate after payroll values, calendar assumptions, 13th-month percentage, or adjustments change.

### what should i check before applying a recommendation?

* employee and payroll group;
* current net taxable and tax withheld;
* lapsed and remaining periods;
* projected 13th Month and remaining 90k space;
* projected tax due and tax gap;
* plus adjustment; and
* the open pay run that will receive the adjustment.

A projection is not a completed payroll result. Applying a recommendation changes the supported open-payroll withholding-tax entry; it does not finalize the payroll or prove the year-end tax result.

### related articles

* generate and review projections
* bulk wtt adjustments
* individual wtt ingestion
* employee 90k
