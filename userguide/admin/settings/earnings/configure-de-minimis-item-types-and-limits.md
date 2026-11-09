# configure De Minimis item types and limits

use De Minimis settings to define a supported benefit, its eligibility, earning method, frequency, payroll destination, and non-taxable ceiling treatment. Assign the saved item to employees through the De Minimis employee workflow.

**navigation:** go to **Settings → Paycheck → De Minimis**.

## how is de minimis different from another non-taxable earning?

De Minimis is a separate product family with prescribed item types, a maximum non-taxable amount, and a recorded taxable excess. A non-taxable allowance or Other Earning uses the general ₱90,000 exemption-ceiling handling shown by those screens. Do not interchange these families only because both can display non-taxable amounts.

the available item choices include:

* Medical Cash Allowance;
* Rice Subsidy;
* Uniform Allowance;
* Medical Assistance;
* Laundry Allowance;
* Achievement Award;
* Holiday Cash Gift;
* Meal Allowance for Overtime and Night Shift; and
* Productivity Incentives.

use only the item whose approved business and reporting meaning matches the benefit.

## before you create an item

* confirm the correct De Minimis type and description;
* identify eligible employees or the applicable rank, department, or employment type;
* confirm the approved amount and current prescribed limit;
* choose the earning method and frequency;
* decide whether eligibility begins on date hired or after a waiting period;
* select the payroll schedule or release month when required; and
* confirm the intended destination shown by the page.

{% hint style="warning" %}
**warning:** do not change the business or tax meaning of an item already used in historical payroll. Use a replacement item when the meaning changes materially.
{% endhint %}

\## which settings control the result?

| level          | setting or record                               | effect                                                                                                                        |
| -------------- | ----------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| company / item | De Minimis definition                           | controls type, applicability, rate method, amount, eligibility start, frequency, schedule, destination, and ceiling treatment |
| employee       | De Minimis assignment                           | connects the item to the employee and stores the supported employee-specific amount and assignment values                     |
| payroll        | pay date, open-payroll state, and recalculation | determines when the eligible assignment is calculated and shown                                                               |

the item definition does not automatically assign the benefit to all employees.

## which earning methods are available?

| method                   | use                                                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------- |
| Fixed Rate               | use the configured fixed amount                                                                                   |
| Daily Rate               | calculate using the configured daily-rate percentage; the current page identifies Average Daily Rate as the basis |
| Prorated By Days Worked  | prorate the amount using days worked                                                                              |
| Prorated By Hours Worked | prorate the amount using hours worked                                                                             |

the page also contains specialized leave-credit behavior for supported monetized-leave records. Use only the options actually displayed for the selected item.

## how do i create a de minimis item?

1. open **Settings → Paycheck → De Minimis**.
2. select **Add De Minimis**.
3. select the **De Minimis Type** and enter a clear description.
4. select **Applicable To**:
   * All Employee;
   * Rank;
   * Department; or
   * Employment Type.
5. complete the displayed group selection when the item is not for all employees.
6. select the **De Minimis Rate Type** and complete its amount, percentage, or proration values.
7. choose the eligibility start:
   * **Date Hired**; or
   * **Start After** a stated number of months or years from date hired.
8. select the frequency. The current workflow supports one-time, per payroll, semi-monthly, monthly, and annual schedules for ordinary items.
9. select the payroll schedule. For annual items, select the release month when requested.
10. confirm the destination:
    * **Add to Non Taxable Income**; or
    * **Less to Taxable Income**.
11. review the complete setup, then select **Save**.

## what happens when the amount exceeds the limit?

the De Minimis workflow stores a maximum non-taxable amount and an excess value. The current page states that an amount above the prescribed limit is categorized as taxable earning.

before payroll approval, review:

* configured amount;
* employee amount;
* maximum non-taxable amount;
* excess amount; and
* resulting payroll and tax output.

## how do i change or retire an item?

open the item detail and use the supported edit or delete action only after reviewing employee assignments and open payroll. Do not delete or rename an item merely to hide it from future use when historical payroll already depends on its meaning.

for a statutory or business-rule change:

1. confirm the effective date;
2. determine whether existing assignments should continue or be replaced;
3. update or create the item according to the approved policy;
4. review affected employee assignments; and
5. recalculate the affected open payroll.

## warnings and troubleshooting

* **No item available for an employee:** confirm the item is active, the employee matches its applicability, and the eligibility waiting period has passed.
* **Unexpected amount:** review rate type, configured amount or percentage, worked days/hours, and employee assignment.
* **Unexpected taxable excess:** compare the amount with the stored maximum non-taxable amount.
* **Annual item missing:** review the selected release month and payroll schedule.
* Downloaded Excel or CSV lists reflect the current settings list; use them for review, not as proof that employee assignments were changed.

## continue in the affected module

* [review de minimis in payroll](../../paycheck/)

### how is De Minimis prorated for an eligible new hire?

this explanation applies when all of these conditions are met:

* the employee is a new hire;
* the employee is monthly-paid;
* the payroll period is semi-monthly;
* **Actual Formula** is enabled; and
* the selected De Minimis method prorates by days worked or hours worked.

Ashima compares worked days or worked hours with all scheduled non-rest workdays across the cutoff. paid leave is not included as worked time in this calculation. dates before the employee's hire date are not treated as regular absences.

use this explanation only for the setup above. it does not describe every De Minimis method, pay type, or payroll schedule.
