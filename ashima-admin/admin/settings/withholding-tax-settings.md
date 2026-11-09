# Withholding tax settings

### Withholding Tax

Use this page to create and maintain withholding-tax deduction schedules used later in payroll.

**Navigation:** Go to **Settings → Pay Check → Taxes → Withholding Tax**

#### What does this page display?

The page displays:

* a withholding-tax schedule listing
* rank options
* detail access for each schedule
* create, update, and delete actions

#### What can I do from this page?

You can:

* create a withholding-tax deduction schedule
* assign the schedule to a selected rank
* set the deduction timing and method
* update or delete an existing schedule

#### Fields

* **Rank (\*)** — required rank selector. The current source expects the rank value to be unique within the withholding-tax schedule list.
* **Description** — optional schedule description.
* **Schedule (\*)** — required deduction schedule.
* **Method (\*)** — required withholding-tax method.

`(*) Required fields must be completed before saving.`

#### What happens after I save?

The withholding-tax schedule becomes available as a company rule used later in payroll computation.

#### Rules, warnings, or behavior notes

* rank is required and must be unique within this schedule setup
* both **Schedule** and **Method** are required
* this page defines deduction schedules, while **Withholding Tax Rule** sets the company computation basis

#### Image Placeholder

\[Image: Withholding Tax page showing the withholding-tax schedule listing and details]

***

### Withholding Tax Rule

Use this page to set the company-level withholding-tax computation basis.

**Navigation:** Go to **Settings → Pay Check → Taxes → Withholding Tax Rule**

#### What does this page display?

The page displays the current company withholding-tax rule and the current default value.

#### What can I do from this page?

You can choose the company-level computation basis the payroll engine should use for withholding tax.

#### What happens after I save?

The company withholding-tax rule is updated, and payroll uses that basis going forward.

#### Rules, warnings, or behavior notes

* if no withholding-tax rule record exists yet, the page inserts a default company setup before rendering
* this page sets the company-wide rule, while the **Withholding Tax** page manages the deduction schedules tied to rank and schedule

#### Image Placeholder

\[Image: Withholding Tax Rule page showing the current computation basis setting]

***

### Withholding Tax Annual

Use this page to review the annual withholding-tax table used by payroll reporting and annual tax references.

**Navigation:** Go to **Settings → Pay Check → Withholding Tax Annual**

#### What does this page display?

The page displays the annual withholding-tax reference table.

#### What can I do from this page?

This is mainly a review page for the annual withholding-tax reference data.

#### Rules, warnings, or behavior notes

* use this page when checking annual tax reference data rather than employee-level payroll setup

#### Image Placeholder

\[Image: Withholding Tax Annual page showing annual tax reference rows]
