# De minimis item types and limits

Use De Minimis settings to define a supported benefit, its eligibility, earning method, frequency, payroll destination, and non-taxable ceiling treatment. Assign the saved item to employees through the De Minimis employee workflow.

**Navigation:**\
go to **Settings → Paycheck → De Minimis**.

## how is de minimis different from another non-taxable earning?

De Minimis is a separate product family with prescribed item types, a maximum non-taxable amount, and a recorded taxable excess. A non-taxable allowance or Other Earning uses the general ₱90,000 exemption-ceiling handling shown by those screens. Do not interchange these families only because both can display non-taxable amounts.

The current item choices include:

* Medical Cash Allowance;
* Rice Subsidy;
* Uniform Allowance;
* Medical Assistance;
* Laundry Allowance;
* Achievement Award;
* Holiday Cash Gift;
* Meal Allowance for Overtime and Night Shift; and
* Productivity Incentives.

Use only the item whose approved business and reporting meaning matches the benefit.

## before you create an item

* confirm the correct De Minimis type and description;
* identify eligible employees or the applicable rank, department, or employment type;
* confirm the approved amount and current prescribed limit;
* choose the earning method and frequency;
* decide whether eligibility begins on date hired or after a waiting period;
* select the payroll schedule or release month when required; and
* confirm the intended destination shown by the page.

> \[!WARNING] Do not change the business or tax meaning of an item already used in historical payroll. Use a replacement item when the meaning changes materially.

## which settings control the result?

| level          | setting or record                               | effect                                                                                                                        |
| -------------- | ----------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------- |
| company / item | De Minimis definition                           | controls type, applicability, rate method, amount, eligibility start, frequency, schedule, destination, and ceiling treatment |
| employee       | De Minimis assignment                           | connects the item to the employee and stores the supported employee-specific amount and assignment values                     |
| payroll        | pay date, open-payroll state, and recalculation | determines when the eligible assignment is calculated and shown                                                               |

The item definition does not automatically assign the benefit to all employees.

## which earning methods are available?

| method                   | use                                                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------- |
| Fixed Rate               | use the configured fixed amount                                                                                   |
| Daily Rate               | calculate using the configured daily-rate percentage; the current page identifies Average Daily Rate as the basis |
| Prorated By Days Worked  | prorate the amount using days worked                                                                              |
| Prorated By Hours Worked | prorate the amount using hours worked                                                                             |

The page also contains specialized leave-credit behavior for supported monetized-leave records. Use only the options actually displayed for the selected item.

## how do i create a de minimis item?

1. Open **Settings → Paycheck → De Minimis**.
2. Select **Add De Minimis**.
3. Select the **De Minimis Type** and enter a clear description.
4. Select **Applicable To**:
   * All Employee;
   * Rank;
   * Department; or
   * Employment Type.
5. Complete the displayed group selection when the item is not for all employees.
6. Select the **De Minimis Rate Type** and complete its amount, percentage, or proration values.
7. Choose the eligibility start:
   * **Date Hired**; or
   * **Start After** a stated number of months or years from date hired.
8. Select the frequency. The current workflow supports one-time, per payroll, semi-monthly, monthly, and annual schedules for ordinary items.
9. Select the payroll schedule. For annual items, select the release month when requested.
10. Confirm the destination:
    * **Add to Non Taxable Income**; or
    * **Less to Taxable Income**.
11. Review the complete setup, then select **Save**.

## what happens when the amount exceeds the limit?

The De Minimis workflow stores a maximum non-taxable amount and an excess value. The current page states that an amount above the prescribed limit is categorized as taxable earning.

Before payroll approval, review:

* configured amount;
* employee amount;
* maximum non-taxable amount;
* excess amount; and
* resulting payroll and tax output.

## how do i change or retire an item?

Open the item detail and use the supported edit or delete action only after reviewing employee assignments and open payroll. Do not delete or rename an item merely to hide it from future use when historical payroll already depends on its meaning.

For a statutory or business-rule change:

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

## related articles

* [employee de minimis assignments](/broken/pages/008391bde093784ebe818f28d77d83c78cd29d5e)
* [earnings items overview](/broken/pages/ef4d970cfc54751933d4ee1de3ad67c41a808216)
* [allowances](/broken/pages/e54bab887f0ee0c152b2ef1a9ace015f28ff7462)
* [other earnings](/broken/pages/c408d5ff58ca0f2aebfa17d6dbc7a71b31f3317c)
* [payroll register](/broken/pages/6bbddef5f8b334eba1ffee39305c12ade382ebe8)
