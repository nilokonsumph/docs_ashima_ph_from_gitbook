# configure withholding-tax schedules and rules

use Withholding Tax settings to maintain the company computation basis, deduction schedule, and supported tax method used with employee tax information and payroll results.

**navigation:** go to **Settings → Paycheck → Withholding Tax** and the related **Withholding Tax Rule** page.

## what are the setting areas?

* **Withholding Tax Rule** defines the company compensation basis used for tax computation.
* **Withholding Tax** defines the schedule and method assigned by the supported company grouping, such as rank.
* **Employee tax information** supplies the employee's applicable tax status or supported fixed-tax setup.
* **Payroll** calculates the employee's tax result using taxable payroll and the applicable setup.

## before you change a tax setting

confirm:

* the approved company tax basis and method;
* the affected rank, group, or employee population;
* employee tax information;
* the effective payroll period;
* open payroll already calculated using the previous setup; and
* the affected tax and year-end reports.

{% hint style="warning" %}
**warning:** a withholding-tax setting change can alter payroll and statutory reporting. Test and review an affected open payroll before broad use.
{% endhint %}

\## how do i update a withholding-tax setting?

1. open the required company tax page.
2. review the current basis, schedule, method, and affected grouping.
3. Update only the approved field.
4. save the setting.
5. Recalculate affected open payroll.
6. Compare employee tax details, masterlist, payslip, and reports.

## what is not changed by a payroll adjustment?

a Withholding Tax Adjustment changes the applicable payroll result. It does not by itself replace the company tax rule, company schedule, or employee tax status.

use the setting page for approved company-rule changes and the supported payroll adjustment for a run-specific correction.

## use Withholding Tax

use this page to create and maintain withholding-tax deduction schedules used later in payroll.

**navigation:** go to **Settings → Pay Check → Taxes → Withholding Tax**

## review saved Withholding Tax records

the page displays:

* a withholding-tax schedule listing
* rank options
* detail access for each schedule
* create, update, and delete actions

## manage Withholding Tax

you can:

* create a withholding-tax deduction schedule
* assign the schedule to a selected rank
* set the deduction timing and method
* update or delete an existing schedule

## complete the Withholding Tax details

* **Rank (\*)** — required rank selector. The current source expects the rank value to be unique within the withholding-tax schedule list.
* **Description** — optional schedule description.
* **Schedule (\*)** — required deduction schedule.
* **Method (\*)** — required withholding-tax method.

`(*) Required fields must be completed before saving.`

## verify the saved Withholding Tax

the withholding-tax schedule becomes available as a company rule used later in payroll computation.

## apply the Withholding Tax rules

* rank is required and must be unique within this schedule setup
* both **Schedule** and **Method** are required
* this page defines deduction schedules, while **Withholding Tax Rule** sets the company computation basis

## use Withholding Tax Rule

use this page to set the company-level withholding-tax computation basis.

**navigation:** go to **Settings → Pay Check → Taxes → Withholding Tax Rule**

## review saved Withholding Tax Rule records

the page displays the current company withholding-tax rule and the current default value.

## manage Withholding Tax Rule

you can choose the company-level computation basis the payroll engine should use for withholding tax.

## verify the saved Withholding Tax Rule

the company withholding-tax rule is updated, and payroll uses that basis going forward.

## apply the Withholding Tax Rule rules

* if no withholding-tax rule record exists yet, the page inserts a default company setup before rendering
* this page sets the company-wide rule, while the **Withholding Tax** page manages the deduction schedules tied to rank and schedule

## use Withholding Tax Annual

use this page to review the annual withholding-tax table used by payroll reporting and annual tax references.

**navigation:** go to **Settings → Pay Check → Withholding Tax Annual**

## review saved Withholding Tax Annual records

the page displays the annual withholding-tax reference table.

## manage Withholding Tax Annual

this is mainly a review page for the annual withholding-tax reference data.

## apply the Withholding Tax Annual rules

* use this page when checking annual tax reference data rather than employee-level payroll setup

## continue in the affected module

* [review withholding tax in payroll](../../paycheck/)
