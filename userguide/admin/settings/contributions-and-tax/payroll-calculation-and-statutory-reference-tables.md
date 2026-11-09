# review payroll calculation and statutory reference tables

**navigation:** go to **Settings → Pay Check**

use the **Pay Check** settings group to build the payroll backbone and the payroll-side type definitions the company uses later in payroll operations.

the Pay Check settings fall into four categories:

**Payroll structure**

* **Pay Schedule** — defines the payroll cadence the company uses
* **Payroll Calendar** — defines the actual payroll dates and calendar periods tied to each schedule
* **Pay Rate** — defines the company pay-rate and related payroll calculation setup
* **Payroll Group** — defines the company pay-rate and related payroll calculation setup

**Payroll entry data types**

* Other earnings
* allowance
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

complete the payroll structure first. Payroll groups, pay-run creation, and pay-period display all depend on Pay Schedule, Payroll Calendar, Pay Rate, and Payroll Group being set up before payroll operations begin.

these pages do not all do the same thing:

* some define the payroll backbone
* some create company-defined payroll-entry types
* some define a default rule the payroll engine follows
* some expose a statutory or reference table used during computation

***

## understand how payroll structure affects pay runs

before payroll can run correctly, the company needs a consistent payroll structure.

the core settings in that backbone are:

* **Pay Schedule** — defines the payroll cadence the company uses
* **Payroll Calendar** — defines the actual payroll dates and calendar periods tied to each schedule
* **Pay Rate** — defines the company pay-rate and related payroll calculation setup
* **Payroll Group** — groups employees into payroll runs and ties them to the relevant payroll cadence and schedule behavior

these settings matter because later payroll actions such as **+ New**, pay-run creation, pay-period display, and payroll grouping all depend on them.

## use Pay Schedule

use this page to define the company pay schedules used by payroll groups and payroll calendars.

**navigation:** go to **Settings → Pay Check → Pay Schedule**

Pay Schedule sets the payroll cadence - weekly, monthly, fortnightly, semi-monthly, or other schedules the company uses. Later payroll setup depends on this page: payroll groups, payroll calendar structure, and payroll-run creation all read from the pay schedules defined here.

use this page to review and maintain the pay schedules that the rest of payroll depends on. the saved pay schedule becomes part of the payroll backbone used later by payroll groups, payroll calendar setup, and payroll run creation.

## apply the Pay Schedule rules

* pay schedule is not just a label. It affects payroll periods, payroll-calendar structure, and downstream payroll behavior
* later payroll setup depends on this page even when the operational payroll actions happen elsewhere

***

## use Payroll Calendar

use this page to define the actual payroll dates and covered periods for each pay schedule.

**navigation:** go to **Settings → Pay Check → Payroll Calendar**

the payroll calendar records become the date framework for payroll run creation and pay-period display. If payroll calendar setup is incomplete, payroll creation and payroll grouping behavior can be affected.

use this page to review and maintain the calendar entries that payroll later uses when determining:

* payroll date
* covered period
* payroll period structure
* schedule-specific pay cycles

the saved payroll-calendar records become the date framework used later by payroll run creation and period display.

## apply the Payroll Calendar rules

* payroll runs later depend on these calendar records to determine valid pay dates and pay periods
* if payroll calendar setup is incomplete, payroll creation and payroll grouping behavior can be affected

***

## use Pay Rate Table

use this page to define the company pay-rate setup used by payroll calculations.

**navigation:** go to **Settings → Pay Check → Pay Rate**

Pay Rate is part of the payroll structure. Pay rates for overtime, holiday premium, rest day pay, night shift differential - refer back to the Pay Rate table when defining premium rate behavior.

## apply the Pay Rate Table rules

* this page is part of the company payroll backbone
* other settings pages can depend on the **Pay Rate** table when defining premium or differential behavior

***

## use Payroll Groups

use this page to create and maintain payroll groups that control which employees are processed together in payroll.

**navigation:** go to **Settings → Pay Check → Payroll Group**

Payroll groups are major company setup records. Pay runs are created per payroll group, so this page directly affects payroll operations. After saving, the payroll group becomes available for employee assignment and payroll processing.

use this page to review and maintain the payroll groups that later affect:

* employee payroll assignment
* pay-run creation
* pay-date and pay-period selection behavior
* default work schedule links in some workflows

Ideally, each payroll group should be limited to around 150 employees.

{% hint style="info" %}
**note:** payroll group is a major company setup record, not just a filter. define your pay groups properly.

later payroll runs are created per payroll group, so this setting directly affects payroll operations
{% endhint %}

the payroll group becomes available for employee assignment and later payroll processing.

## apply the Payroll Groups rules

* payroll group is a major company setup record, not just a filter
* later payroll runs are created per payroll group, so this page directly affects payroll operations

## use PhilHealth Tables

use this page to review the active PhilHealth contribution table the system uses during payroll computation.

**navigation:** go to **Settings → Pay Check → PhilHealth Tables**

this is a reference page. It exposes the active statutory table payroll reads when computing PhilHealth contributions. This page is not the employee assignment page for PhilHealth. Changes to statutory tables affect contribution output downstream — handle them carefully.

## use HDMF Tables

use this page to review the active HDMF contribution table used by payroll.

**navigation:** go to **Settings → Pay Check → HDMF Tables**

this is a reference page for the contribution table the system reads during payroll. Payroll can show more than one HDMF-related output line, but this page is the company-level reference view for the contribution table itself.
