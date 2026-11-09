# Paycheck settings

**Navigation:** Go to **Settings → Pay Check**

Use the **Pay Check** settings group to build the payroll backbone and the payroll-side type definitions the company uses later in payroll operations.

The Pay Check settings fall into four categories:

**Payroll structure**

* **Pay Schedule** — defines the payroll cadence the company uses
* **Payroll Calendar** — defines the actual payroll dates and calendar periods tied to each schedule
* **Pay Rate** — defines the company pay-rate and related payroll calculation setup
* **Payroll Group** — defines the company pay-rate and related payroll calculation setup

**Payroll entry data types**

* Other earnings
* Allowance
* **Government Loans** — government-loan types for employee assignment
* **Third-Party Loans** — private or company-recognized loan types
* **Insurance** — insurance deduction types with recurrence setup
* **Other Deductions** — company-specific deduction types

**Tax rules**

* **Withholding Tax** — withholding-tax deduction schedules by rank
* **Withholding Tax Rule** — the company withholding-tax computation basis

**Statutory reference tables**

* **Withholding Tax Annual** — annual withholding-tax reference data
* **PhilHealth Tables** — active PhilHealth contribution table
* **HDMF Tables** — active HDMF contribution table

Complete the payroll strucure first. Payroll groups, pay-run creation, and pay-period display all depend on Pay Schedule, Payroll Calendar, Pay Rate, and Payroll Group being set up before payroll operations begin.

These pages do not all do the same thing:

* some define the payroll backbone
* some create company-defined payroll-entry types
* some define a default rule the payroll engine follows
* some expose a statutory or reference table used during computation

***

### What should administrators know about the payroll structure settings?

Before payroll can run correctly, the company needs a consistent payroll structure.

The core settings in that backbone are:

* **Pay Schedule** — defines the payroll cadence the company uses
* **Payroll Calendar** — defines the actual payroll dates and calendar periods tied to each schedule
* **Pay Rate** — defines the company pay-rate and related payroll calculation setup
* **Payroll Group** — groups employees into payroll runs and ties them to the relevant payroll cadence and schedule behavior

These settings matter because later payroll actions such as **+ New**, pay-run creation, pay-period display, and payroll grouping all depend on them.

#### Pay Schedule

Use this page to define the company pay schedules used by payroll groups and payroll calendars.

**Navigation:** Go to **Settings → Pay Check → Pay Schedule**

Pay Schedule sets the payroll cadence - weekly, monthly, fortnightly, semi-monthly, or other schedules the company uses. Later payroll setup depends on this page: payroll groups, payroll calendar structure, and payroll-run creation all read from the pay schedules defined here.

Use this page to review and maintain the pay schedules that the rest of payroll depends on.\
\
The saved pay schedule becomes part of the payroll backbone used later by payroll groups, payroll calendar setup, and payroll run creation.

#### Rules, warnings, or behavior notes

* pay schedule is not just a label. It affects payroll periods, payroll-calendar structure, and downstream payroll behavior
* later payroll setup depends on this page even when the operational payroll actions happen elsewhere

***

#### Payroll Calendar

Use this page to define the actual payroll dates and covered periods for each pay schedule.

**Navigation:** Go to **Settings → Pay Check → Payroll Calendar**

The payroll calendar records become the date framework for payroll run creation and pay-period display. If payroll calendar setup is incomplete, payroll creation and payroll grouping behavior can be affected.

Use this page to review and maintain the calendar entries that payroll later uses when determining:

* payroll date
* covered period
* payroll period structure
* schedule-specific pay cycles

The saved payroll-calendar records become the date framework used later by payroll run creation and period display.

#### Rules, warnings, or behavior notes

* payroll runs later depend on these calendar records to determine valid pay dates and pay periods
* if payroll calendar setup is incomplete, payroll creation and payroll grouping behavior can be affected

***

#### Pay Rate Table

Use this page to define the company pay-rate setup used by payroll calculations.

**Navigation:** Go to **Settings → Pay Check → Pay Rate**

Pay Rate is part of the payroll structure. Pay rates for overtime, holiday premium, rest day pay, night shift differential - refer back to the Pay Rate table when defining premium rate behavior.

#### Rules, warnings, or behavior notes

* this page is part of the company payroll backbone
* other settings pages can depend on the **Pay Rate** table when defining premium or differential behavior

####

***

#### Payroll Groups

Use this page to create and maintain payroll groups that control which employees are processed together in payroll.

**Navigation:** Go to **Settings → Pay Check → Payroll Group**

Payroll groups are major company setup records. Pay runs are created per payroll group, so this page directly affects payroll operations. After saving, the payroll group becomes available for employee assignment and payroll processing.

Use this page to review and maintain the payroll groups that later affect:

* employee payroll assignment
* pay-run creation
* pay-date and pay-period selection behavior
* default work schedule links in some workflows

Ideally, each payroll group should be limited to around 150 employees.

{% hint style="info" %}
payroll group is a major company setup record, not just a filter. define your pay groups properly.

later payroll runs are created per payroll group, so this setting directly affects payroll operations
{% endhint %}

The payroll group becomes available for employee assignment and later payroll processing.

#### Rules, warnings, or behavior notes

* payroll group is a major company setup record, not just a filter
* later payroll runs are created per payroll group, so this page directly affects payroll operations

#### Image Placeholder

\[Image: Payroll Group page showing payroll-group list and payroll-group setup controls]

***

####

####

#### Government Loans

Use this page to create and maintain the government-loan types your company can assign to employees.

**Navigation:** Go to **Settings → Pay Check → Deductions → Government Loans**

#### What does this page display?

The page shows a searchable list of saved government-loan types with autosuggest support, a detail page for each type, and create, update, and delete actions. Employee-group targeting options — Rank, Department, and Employment Type — are also available.

#### Fields

* **Loan Type (\*)** — the government-loan type name.
* **Applicable For** — the employee group the type applies to.
* **Rank** — optional rank targeting.
* **Department** — optional department targeting.
* **Employment Type** — optional employment-type targeting.

`(*) Required fields must be completed before saving.`

This page creates the reusable loan type only. The actual employee assignment happens later in employee payroll setup. Target selections control where the type can be used.

#### Image Placeholder

\[Image: Government Loans page showing loan-type list, autosuggest search, and create flow]

***

### Third-Party Loans

Use this page to create and maintain third-party loan types that can be assigned to employees.

**Navigation:** Go to **Settings → Pay Check → Deductions → Third-Party Loans**

#### What does this page display?

The page shows a searchable list of third-party loan types, a loan detail page, and create, update, and delete actions.

#### Fields

* **Loan Type (\*)** — the third-party loan type name.
* **Description** — optional description.

`(*) Required fields must be completed before saving.`

This page creates the loan type only. Employee-level assignment happens later in payroll setup. Delete a loan type only after confirming it is not already used in employee records.

#### Image Placeholder

\[Image: Third-Party Loans page showing loan-type listing and details access]

***

### Insurance

Use this page to create and maintain insurance deduction types that can be assigned to employees.

**Navigation:** Go to **Settings → Pay Check → Deductions → Insurance**

#### What does this page display?

The page shows a searchable insurance list, an insurance detail page, and create, update, and delete actions.

#### Fields

* **Insurance Name (\*)** — the provider or insurance name. Must be unique among active records.
* **Insurance Type (\*)** — the insurance category. Selecting `others` requires an additional value.
* **Other Insurance Type** — required when Insurance Type is set to `others`.
* **Plan Details** — optional plan information.
* **Deduction Amount (\*)** — numeric amount with up to 2 decimal places.
* **Recurring Payment (\*)** — controls whether the deduction runs once or repeats.
* **Recurring Type** — required when recurring is enabled. Controls whether the schedule runs by interval or by occurrence.
* **Deduction Schedule** — required for interval-based recurring deductions.
* **Payroll Schedule** — required for recurring deduction timing.
* **Start Date (\*)** — required for both recurring and one-time setups.
* **End Date** — required for interval-based recurring deductions.
* **Number of Occurrence** — required for occurrence-based recurring deductions.

`(*) Required fields must be completed before saving.`

The required fields change depending on whether the deduction is one-time, interval-based recurring, or occurrence-based recurring. After saving, the insurance type becomes available as a reusable payroll deduction setting for employee assignment.

#### Image Placeholder

\[Image: Insurance settings page showing insurance list and deduction scheduling fields]

***

### Other Deductions

Use this page to create and maintain company-specific deduction types outside of loans and insurance.

**Navigation:** Go to **Settings → Pay Check → Deductions → Other Deductions**

#### What does this page display?

The page shows a searchable list of other deduction types with autosuggest support, employee-group targeting options (Rank, Department, Employment Type), and create and delete actions.

#### Fields

* **Deduction Name (\*)** — the deduction type name. Must be unique among active company deduction records.
* **Deduction Amount (\*)** — numeric amount with up to 2 decimal places.
* **Applicable For (\*)** — the scope or employee grouping the deduction applies to.
* **Recurring (\*)** — controls whether the deduction is one-time or recurring.
* **Recurring Type** — required when recurring is enabled.
* **Occurrence Start Date** — required for one-time or occurrence-based setup.
* **Interval Schedule** — required for interval-based recurring setup.
* **Payroll Schedule** — required for interval-based or occurrence-based recurring setup.
* **Interval Start Date** — required for interval-based setup.
* **Interval End Date** — required for interval-based setup.
* **Number of Occurrence** — required for occurrence-based setup.
* **Occurrence Schedule** — required for occurrence-based setup.
* **Rank** — optional rank targeting.
* **Department** — optional department targeting.
* **Employment Type** — optional employment-type targeting.
* **Description** — optional notes.

`(*) Required fields must be completed before saving.`

One-time and recurring setups use different required fields. This page defines the deduction type only — it does not deduct from an employee until the type is used in employee payroll configuration.

#### Image Placeholder

\[Image: Other Deductions page showing deduction list and recurring setup fields]

***

### Withholding Tax

Use this page to create and maintain withholding-tax deduction schedules used in payroll.

**Navigation:** Go to **Settings → Pay Check → Taxes → Withholding Tax**

#### What does this page display?

The page shows a withholding-tax schedule listing by rank, detail access for each schedule, and create, update, and delete actions.

#### Fields

* **Rank (\*)** — required rank selector. Must be unique within the withholding-tax schedule list.
* **Description** — optional schedule description.
* **Schedule (\*)** — required deduction schedule.
* **Method (\*)** — required withholding-tax method.

`(*) Required fields must be completed before saving.`

After saving, the schedule becomes a company rule used in payroll computation. This page manages deduction schedules by rank. The **Withholding Tax Rule** page sets the company-wide computation basis.

#### Image Placeholder

\[Image: Withholding Tax page showing the withholding-tax schedule listing and schedule details]

***

### Withholding Tax Rule

Use this page to set the company-level withholding-tax computation basis used by payroll.

**Navigation:** Go to **Settings → Pay Check → Taxes → Withholding Tax Rule**

#### What does this page display?

The page shows the current company withholding-tax rule and its current default value.

After saving, payroll uses the updated computation basis going forward. If no withholding-tax rule record exists yet, the page creates a default company setup before rendering. This page sets the company-wide rule. The **Withholding Tax** page manages the deduction schedules tied to rank and schedule.

#### Image Placeholder

\[Image: Withholding Tax Rule page showing the current computation basis setting and save control]

***

### Withholding Tax Annual

Use this page to review the annual withholding-tax reference table used by payroll reporting.

**Navigation:** Go to **Settings → Pay Check → Withholding Tax Annual**

This is a reference page. Use it when checking annual tax reference data rather than employee-level payroll setup.

#### Image Placeholder

\[Image: Withholding Tax Annual page showing annual tax reference rows]

***

### PhilHealth Tables

Use this page to review the active PhilHealth contribution table the system uses during payroll computation.

**Navigation:** Go to **Settings → Pay Check → PhilHealth Tables**

This is a reference page. It exposes the active statutory table payroll reads when computing PhilHealth contributions. This page is not the employee assignment page for PhilHealth. Changes to statutory tables affect contribution output downstream — handle them carefully.

#### Image Placeholder

\[Image: PhilHealth Tables page showing the active PhilHealth contribution rows]

***

### HDMF Tables

Use this page to review the active HDMF contribution table used by payroll.

**Navigation:** Go to **Settings → Pay Check → HDMF Tables**

This is a reference page for the contribution table the system reads during payroll. Payroll can show more than one HDMF-related output line, but this page is the company-level reference view for the contribution table itself.

#### Image Placeholder

\[Image: HDMF Tables page showing the active HDMF contribution table]
