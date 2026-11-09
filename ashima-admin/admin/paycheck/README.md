# Paycheck

the **Paycheck** module is where administrators create, review, and manage payroll runs in the Admin Portal.

use this module to move payroll from draft pay run through approval, payment processing, and payslip release. the module also gives access to the earnings, deductions, contribution, and withholding tax pages that support payroll calculations.

payroll in ashima follows three stages:

1. **payroll input** — create the pay run, review employee-level payroll values and recalculate if needed.
2. **preview & approve** — review the consolidated payroll output (masterlist), exclusions, adjustments, and approval readiness.
3. **process payment** — handle bank file output, payslip generation, and payslip release after payroll is closed.



#### before you begin: key payroll terms

* [**payroll group**](../settings/paycheck-settings.md#payroll-groups) - the employee group included in one pay run.
* **pay date** - the scheduled payroll payment date.
* **pay period** - the date range covered by the payroll calculation. this determines which attendance, leave, earnings, deductions, and payroll changes are included in the run.
* [**pay schedule**](../settings/paycheck-settings.md#pay-schedule) - the payroll frequency used by the payroll group, such as semi-monthly.
* **pay run** - start new pay runs, review open pay runs, switch to submitted or closed payroll.&#x20;
* **pay run details** - employee payroll summary for one selected pay run — review values and recalculate&#x20;
* [**masterlist**](./#payroll-masterlist) - the consolidated payroll review page for all pay runs that belong to the same pay date and pay period.
* **payroll exclusion**  - exclude or include employees from the current payroll output&#x20;
* **adjustment -** add direct payroll corrections to the current pay run&#x20;
* **pay run freeze** - admin-controlled payroll freeze used while payroll is being finalised&#x20;
* [**post payroll adjustment (ppa)**](./#what-are-post-payroll-adjustments-ppa), used for eligible late payroll corrections after the original payroll is no longer open for normal review.
* Recalculation

{% hint style="info" %}
Use the pay schedule to understand how often a group is paid, the pay period to confirm what is included in the run, and the pay date to confirm when payment is due.
{% endhint %}

### what pages are available in the paycheck module?

the main navigation links under **Pay Check** are:

* [**pay run** ](./#pay-runs)— the starting point for all payroll processing
* [**earnings**](pay-items-and-statutory-review/earnings.md) — employee compensation setup and earning assignments
* [**deductions**](pay-items-and-statutory-review/deduction.md) — employee loan, insurance, and other deduction assignments
* [**contribution**](./) — statutory contribution review and remittance tracking
* [**withholding tax**](pay-items-and-statutory-review/withholding-tax.md) — withholding tax deduction schedules
* [**pay run freeze**](./#how-do-i-use-freeze-pay-run) — controls for freezing payroll-affecting changes
* **pay run tools** — additional payroll utilities

**year End** and **surfacing** are separate payroll areas accessed from the Pay Run workspace tabs. they are documented as separate workflows.

## pay runs

### what are pay runs?

a **pay run** (often called a _payroll run_) is the scheduled process of calculating and processing employee pay for a specific period.

a pay run typically refers to the full workflow that includes:

* **collecting payroll inputs** such as hours worked, overtime, leave, earnings, and deductions
* **calculating gross pay** based on compensation rules and pay schedules
* **applying deductions and taxes** (e.g., statutory contributions, withholding taxes, etc.)
* **generating net pay** (take-home pay for employees)
* **producing payroll outputs** such as payslips, masterlist and reports
* **finalizing and approving payroll** before bank files are generated for payment

in simpler terms, a pay run is **one complete cycle of processing employee salaries for a defined pay period**, from computation to final payout.

### where can I view my pay runs?

**navigation:**\
Go to **Pay Check → pay run**\
\
there are two ways to view your pay runs, depending on their status:

* **draft pay runs**\
  displays pay runs that are **open** or **rejected**.  \
  \
  draft pay runs are payrolls that are still being prepared. use this area to review entries, manage included or excluded employees, and finalize before approval or closing.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 8.00.12 AM.png" alt=""><figcaption></figcaption></figure>



* **pay run history**\
  displays pay runs that are **pending approval** or **approved/closed**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-24 at 2.44.49 PM.png" alt=""><figcaption></figcaption></figure>

### how do I switch from viewing open pay runs to submitted or closed payroll?

use the **filter** button at the top of the page to switch between these views.

the pay run listing table can be filtered to display either all open and rejected pay runs, or all pending approval and approved/closed pay runs. to change the view, click the filter buttons for **“**<mark style="color:$primary;">**Waiting for Approval / Closed Payroll.**</mark>**”** or switch back to the default view, **“**<mark style="color:$success;">**Open / Rejected Payroll**</mark>**”**

The pay run table listing displays:

* **Pay Run ID**
* **Payroll Group & Pay Schedule**
* **Pay Date**
* **Pay Period**
* **Payroll Cost & Included/Excluded**
* **Status**
* **Action**

### what happens after I switch the view?

the page changes from the open payroll workspace to the pay run history view.

use this view to:

* check submitted payroll
* review pending approval payroll
* review rejected payroll
* review closed payroll

### what do the pay run status values mean?

* **open** - the pay run is still under active payroll review.
* **waiting for approval** -the pay run has already been submitted and is no longer in normal open review.
* **rejected** - the pay run was rejected and should be reviewed, corrected, and submitted again if needed.
* **closed** - the payroll has been approved and moved to closed-payroll actions.

### how do I filter or search this page?

use the top filters when you want to narrow the listing.

* **select employee** narrows the list to a specific employee context&#x20;
* **select pay run ID** narrows the list to a specific payrun&#x20;
* **pay date** narrows the list to a specific payroll date
* **search** applies the selected filters

***

### how do I run a new payroll?

use **+ new** to begin a new payroll run. the two decisions that define the pay run are the **payroll group** and the **pay date**.

the payroll group determines which employees are included. the pay date determines which pay period is used -when you select a pay date, the system displays the corresponding pay period automatically.

**navigation:** go to **pay check → pay run → + new**

#### steps

1. go to **pay check → pay run**.
2. click **+ new**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 3.16.54 PM.png" alt=""><figcaption></figcaption></figure>



3. in **select payroll group**, choose the payroll group you want to run.
4. In **choose payroll date**, select the pay date for the payroll you want to process.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 3.20.00 PM.png" alt=""><figcaption></figcaption></figure>



5. review the pay period the system displays for that pay date.
6. review the employee listing for the selected payroll group.
7. click **done** to continue to the pay run workflow.

{% hint style="info" %}
#### Required fields must be completed before continuing.

* **Choose Payroll Group (\*)** - selects the payroll group for the new pay run. This determines which employees are pulled into the run.
* **Choose Payroll Date (\*)** - selects the pay date and displays the corresponding pay period.
{% endhint %}



***

### can I run pay runs for multiple payroll groups within the same pay period?y

yes. you can create pay runs for one payroll group at a time, and multiple payroll groups can exist within the same pay period.

each pay run is created for a single payroll group only. however, this does not limit you to just one payroll group per pay period. if several payroll groups share the same pay period, you can generate separate pay runs for each group under that same period.

**example:**\
if your pay date is **March 25**, you can run one or more payroll groups that are scheduled to be paid on March 25. Each payroll group will have its own separate pay run, even though they belong to the same pay period.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 3.25.35 PM.png" alt=""><figcaption></figcaption></figure>

***

### how do I delete an open draft pay run?

Use **delete** only when you are sure the draft pay run should no longer be used.

**Navigation:**\
Go to **Pay Check → pay run**

{% hint style="info" %}
&#x20;Delete only applies to open draft pay runs. You will not be able to delete closed/approved pay runs.
{% endhint %}

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 3.31.57 PM.png" alt=""><figcaption></figcaption></figure>

#### steps

1. select the checkbox beside the draft pay run.
2. click **delete**.
3. review the pay run ID shown in the warning.
4. confirm the deletion.

#### what happens after I delete a draft pay run?

the selected open draft pay run is removed from the current payroll review list.

{% hint style="info" %}
#### Rules&#x20;

* ddelete only applies to open draft pay runs.
* deleting a pay run cannot be undone.
* review the pay run ID, pay date, and pay period before confirming.<br>
{% endhint %}

***

## how do I use freeze pay run?

use **freeze pay run** to lock employee and manager payroll changes while you prepare the pay run for approval. this prevents new timesheet, leave, or shift adjustments from affecting the payroll you are currently reviewing.

**navigation:** go to **pay check → pay run lock**

when the freeze is enabled:

* Employees cannot file payroll-affecting adjustments.
* Managers cannot initiate or approve payroll-affecting adjustments.
* Changes tied to timesheets, shifts, and leaves are paused for the duration of the lock period.

the pay run workspace also shows a lock indicator. the page tooltip and helper text display this as **freeze pay run updates** and show whether the pay run is currently **locked** or **unlocked**.

use this function during controlled payroll processing windows, especially before running final approval.

turn it off after payroll has already been finalized, approved, or closed, if the freeze is no longer needed.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 3.36.16 PM.png" alt=""><figcaption></figcaption></figure>



#### what can I do from this page?

* turn the freeze on
* turn the freeze off
* check whether payroll updates are currently locked or unlocked

#### what happens when freeze pay run updates is enabled?

when the freeze is enabled:

* employees can no longer file payroll-affecting changes through the normal update flows
* managers can no longer initiate or approve payroll-affecting changes through the normal approval flows
* timesheet, shift, leave, and similar payroll-impacting requests are temporarily suspended while payroll is being finalized
*

    <figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 3.37.39 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
#### rules:&#x20;

* this is an admin-controlled freeze, not the same as the system-generated **Locked for payroll processing** status.
* use this during controlled payroll finalization windows.
* turn it off after payroll has already been finalized, approved, or closed, if the freeze is no longer needed.
{% endhint %}



***

## pay run details

use the **pay run details** page to review employee-level payroll output for one selected pay run before moving to the masterlist.

**navigation:**\
go to **pay check → pay run → view details**

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 3.40.50 PM.png" alt=""><figcaption></figcaption></figure>

#### what does this page display?

the page shows:

* the selected pay run header
* pay run ID, pay date, payroll period, and status
* related open pay runs in the side summary area
* quick links for **masterlist** and **exclusion**
* the employee payroll summary table

the employee payroll summary table displays:

* employee details
* base pay
* taxable pay
* non taxable pay
* total deductions
* net pay

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 8.14.40 AM.png" alt=""><figcaption></figcaption></figure>

#### what can I do from this page?

* review  [**details of your pay run**](./#how-can-i-view-details-of-my-pay-run)
* update [**open shift hours**](./#how-do-i-update-open-shift-hours-for-this-pay-run)
* run [**recalc**](./#how-do-i-review-and-recalculate-payroll-on-the-pay-run-details-page)
* review [**recalculation history**](./#how-do-i-review-recalculation-history)
* continue to [masterlist](./#payroll-masterlist)

### how can i view details of my pay run?

payroll review follows a top-down path. start from the pay run list, then work down into the employee level.\
\
_<mark style="color:violet;">**step 1  - pay run list**</mark>_ \
\
the Pay Run list shows all open pay runs for the company. each row represents one pay run for one payroll group and pay date. open a pay run by clicking &#x76;_&#x69;ew details_ from the action link.\
\
if you are running several pay groups on the same pay date you will see all of the groups listed on the left most side of the page.\
\
toggle from one pay group to another by clicking on the individual pay run boxes on the left side.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 4.09.49 PM.png" alt=""><figcaption></figcaption></figure>

_<mark style="color:violet;">**step 2  pay run details: employee summary table**</mark>_ \
\
this page shows the employee payroll summary for the selected pay run - one row per employee with their base pay, taxable pay, non-taxable pay, total deductions, and net pay totals.\
\
use &#x73;_&#x65;lect employee name_ and click _search_ to narrow the table to one employee.<br>

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 2.47.05 PM.png" alt=""><figcaption></figcaption></figure>

_<mark style="color:violet;">**step 3  - review individual employee pay**</mark>_ \
\
from the employee summary table, there are two ways to review the payroll breakdown for a specific employee:



*   _**quick view pop-up**_

    Click the _Net Pay_ value in the summary table. This opens a pop-up with similar pay details content without leaving the Pay Run Details page. Use this for a fast check of one employee's breakdown when you do not need to go into the full Pay Details view.<br>

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 1.50.36 PM (2).png" alt=""><figcaption></figcaption></figure>



*   _**full pay details page**_

    click the _employee name_ in the summary table. this opens the full &#x65;_&#x6D;ployee pay details_ page for that employee, showing a complete breakdown of earnings, deductions, contributions, and withholding tax across the payroll run. Use this when you need to review the full payroll result line by line, explain a specific amount to the employee, or investigate a discrepancy before recalculating.<br>

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 2.26.47 PM (1).png" alt=""><figcaption></figcaption></figure>



both paths show the same underlying payroll content - the difference is the depth of navigation. Use the employee name link when you need to work through the detail carefully. Use the Net Pay link when you need a quick reference check.

{% hint style="info" %}
there are two ways to review an employee's payroll breakdown from this page -  the quick view pop up or the full pay details pate.  use the one that fits what you need.
{% endhint %}

***

## updating open shifts on pay run

### how do I update open shift hours for this pay run

configure the open shift settings if your company has employees assigned to open shifts.

if not, you may skip this step.\
\
use **update open shift hours** to correct the total hours for employees assigned to open shifts.

complete this step before proceeding with the payroll run.

**navigation:**\
go to **pay check → pay run → view details**

#### steps

1. click **update open shift hrs**.
2. review the warning shown in the modal.
3. enter the value in **Number of Hours**.

**number of hours (\*)** — records the total open shift hours for the selected pay run.

note that changing total open shift hours may affect the pay of employees who already have approved overtime for the selected pay period. review carefully before updating.

4. click **update**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 3.53.24 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
changing total open shift hours may affect the pay of employees who already have approved overtime for the selected pay period. review carefully before saving.
{% endhint %}

#### what are open shifts?

open shift is a work schedule type used for employees who are not paid against a fixed daily start and end time. when an employee’s effective shift for a date is open whift, ashima processes that date using open-shift rules instead of regular fixed-time shift rules.

open shift is resolved by the employee’s effective shift assignment for the date. \
\
if a different shift is assigned for another date, ashima can use that other shift for that date instead.\
\
more about open shifts on the shift module.&#x20;

#### what does the open shift hours field do when creating a pay run?

when you open a new pay run, ashima checks whether the selected payroll group includes employees whose effective shift is open shift during the covered pay period. If yes, the pay run shows an Open Shift total-hours field.

\
use this field to enter the required total open shift hours for that payroll period. this gives payroll the period-level total to use for employees on open shift.

{% hint style="info" %}
If no employees in the selected pay run are on Open Shift, you can skip this.
{% endhint %}

#### what happens after I update open shift hours?

the pay run uses the updated open shift hour value in the current payroll review.

####

#### what if I leave open shift hours blank?

\
if you leave the Open Shift hours field blank, ashima saves the required open shift hours for that pay run as 0.

this does not automatically mean the employee will receive zero pay. the system can still calculate payroll using the employee’s recorded open shift hours and applicable holiday or pay entitlements.

what changes is that the pay run will no longer use a positive required open Shift total for the payroll period.

in practice, this means:

* the system can still read and total the employee’s open shift logs
* the system does not apply the intended open shift required-hours target for that cutoff
* the system does not apply the same open shift hours cap or comparison logic that would apply if a valid total had been entered
* undertime tied to missing required Open Shift hours may not be computed as intended

\
the main risk is not that payroll stops completely. the main risk is that payroll may be calculated without the correct open shift period target, which can lead to inaccurate payroll results.

{% hint style="info" %}
Best practice: If the pay run includes employees assigned to Open Shift, enter the correct total required hours for the pay period before continuing payroll review.
{% endhint %}



***

## payroll recalculation

### how do I review and recalculate payroll on the pay run details page?

use this page when you need to check employee totals and make sure payroll is fully recalculated before continuing.

**navigation:**\
go to **pay check → pay run → view details**

#### steps

1. open the selected pay run through **view details**.
2. review the employee summary table.
3. use **select employee name** and **search** if you need to narrow the table.
4. click **recalc history** if you want to check previous recalculation activity.
5. click **recalc** if payroll values need to be refreshed.
6. continue only after the employee rows and values are fully loaded.

#### what happens after I use recalc?

the system refreshes payroll values for the current pay run using the latest payroll-affecting data.

on first access, the page may prompt recalculation while payroll details are being prepared.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 4.03.15 PM.png" alt=""><figcaption></figcaption></figure>



the first recalculation can take longer because the system may still be preparing payroll details for the selected group and period.

larger payroll groups can take longer because payroll entries are processed in batches.

keep the page open while recalculation is running.



<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 12.41.23 AM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 10.25.52 AM.png" alt=""><figcaption></figcaption></figure>



{% hint style="info" %}
if the pay run opens but the employee table is empty even though employees belong to the payroll group, click **recalc**.
{% endhint %}



#### why is recalculation important in an open pay run?

recalculation refreshes the pay run so it uses the latest approved and saved payroll data.

an open pay run is not static. while it is still open, payroll-affecting changes can continue to happen.&#x20;

because of this, the figures you first saw on screen may no longer be the latest figures.

in ashima several  page prompts users to recalculate so that all pay entries have been recalculated and recent updates have been accounted for, and warns that continuing without recalculation can result in discrepancies.&#x20;

#### when should I recalculate a pay run?

recalculate when:

* you are opening the pay run for the first time and the details are still loading
* changes may have happened after you last reviewed the page
* you or another admin updated payroll-related data
* the page prompts you to recalculate before continuing

As a best practice, recalculate before you release a pay draft, continue your final review, or submit payroll for approval.

#### what happens if I skip recalculation?

if you continue without recalculating, the pay run may still display older figures.

this can lead to:

* outdated employee pay summaries
* draft payslips that do not reflect the latest updates
* payroll review or approval based on figures that are no longer current

in short, skipping recalculation increases the risk of payroll discrepancies.

#### why does the system prompt recalculation?

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 10.26.30 AM.png" alt=""><figcaption></figcaption></figure>

the prompt appears because the system is checking whether the pay run may have updates that need to be applied before you continue.

this is common in open payroll because payroll data can still move while the pay run is under review.

#### why can recalculation take time

recalculation may take a few minutes, especially for larger payroll groups or pay runs with many updates.

keep the page open until the process finishes so the pay run can fully refresh.

{% hint style="info" %}
best practice: if the pay run is still open and there is any chance that payroll-affecting changes were made after your last review, recalculate first. this helps make sure the pay run, pay draft, and approval review are based on the latest payroll data
{% endhint %}

### how do I review recalculation history?

\
use **recalc history** to see who performed recalculations for the pay run and when.

1. click **recalc History**.
2. review the history table in the modal.

use this when you need to confirm that a recalculation was completed and by whom before moving forward.

#### what does recalculation history show?

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-25 at 4.02.59 PM (1).png" alt=""><figcaption></figcaption></figure>

\
the history shows who recalculated the pay run and when.\
\
it includes:

* who triggered the recalculation
* the payroll group or employee tied to the recalculation record
* the date and time of the recalculation<br>

***

## payroll masterlist

the **payroll masterlist** is the consolidated payroll review page for a selected pay date and payroll period. All pay runs that belong to the same pay date and period are reviewed together at this stage as one payroll output.

use the masterlist to confirm payroll values, manage adjustments and exclusions, check for pay updates, and submit payroll for approval.

**navigation:**\
go to **pay check → pay run → view payroll masterlist**



### how do I move from pay run details to the payroll masterlist?

when you are done reviewing the pay run details, click **continue to masterlist**.

the system may ask whether you want to recalculate before continuing. this prompt appears because payroll-affecting changes can happen while the page is open.

* if you have had the page open for a while, or if you expect changes have been made, choose **recalculate before continuing to masterlist**.
* if you just recalculated and no new changes were made, choose **no need. skip recalculation**.

if you choose to recalculate, keep the page open until the process is complete. the system shows a progress window while it prepares the updated pay run.

#### steps

1. review the pay run details table.
2. click **continue to masterlist**.
3. if prompted, choose whether to recalculate before continuing.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 12.23.17 PM.png" alt=""><figcaption></figcaption></figure>



the system moves you to **payroll masterlist** for the selected pay date and pay period.

{% hint style="info" %}
#### Notes:

* if the page has been open for a while, or you expect payroll-affecting changes have happened, choose the recalculation option before continuing.
* if you recently recalculated and no new changes were made, you can use **No Need. Skip Recalculation**.
{% endhint %}



### what does the masterlist table show?

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 12.21.29 PM.png" alt=""><figcaption></figcaption></figure>



the table shows a payroll summary for each employee:

* **employee details**
* **payroll group**
* **total gross pay**
* **total taxable pay**
* **total non taxable pay**
* **total withholding tax**
* **total deductions**
* **net pay**

### what do the top counters mean?

the summary cards show:

* **status** — the current state of the payroll review, such as **Open**
* **pay date** — the scheduled payroll payment date
* **period from** — the start date of the payroll period
* **period to** — the end date of the payroll period
* **total net pay** — the current total net pay for all employees included in the masterlist

confirm all five values before continuing to make sure you are reviewing the correct payroll set.



### what can I do from this page?

* search the masterlist by employee.  how do I search the masterlist?
  1. In **Select Employee Name**, choose the employee you want to review.
  2. Click **Search**.
* review the green and red light **P (payroll)** and **T (timesheet)** indicators
* run **check for pay updates**
* open **paycheck adjustment**
* open **exclusion**
* send a **Pay Draft**
* submit **payroll for approval**
* **download** the masterlist

###

### how do I search the masterlist?

Use **Select Employee Name** and click **Search** to narrow the masterlist to one employee.

###

### what should administrators know about the <mark style="color:$success;">green</mark> and <mark style="color:$danger;">red</mark> light indicators on the masterlist?

the <mark style="color:$success;">green</mark> and <mark style="color:$danger;">red</mark> light **P (payroll)** and **T (timesheet )** indicators are payroll readiness checks on the masterlist page.

* **P** (Pay Update Check) - identifies payroll-affecting changes that may require recalculation before approval.
* **T** (Timesheet Check) - identifies timesheet-related payroll changes that still need attention before approval.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 12.21.29 PM (1).png" alt=""><figcaption></figcaption></figure>

the page runs these checks automatically when the masterlist opens. you can run them again using **check for pay updates**.

when both indicators are green, the current check found no items requiring recalculation. \
\
when **P** or **T** is red, the system found employees whose payroll details still need to be recalculated before submission. \
\
**submit for approval** is disabled until both indicators return to green.

### what **usually turns the indicators red?**

the check turns red when it detects payroll-affecting updates that have not yet been fully refreshed into the current payroll state. This can include changes to:

* hours worked, tardiness, undertime, or absences
* paid leave, rest day or holiday premium, overtime, or night shift differential
* allowances, commissions, De Minimis, or other earnings
* government loans, other deductions, or retroactive pay
* third party loans
* retroactive pay

### how do I clear a <mark style="color:$danger;">red indicator?</mark>

1. click **check for pay updates**.
2. review the employees flagged by the system.
3. recalculate the payroll.
4. run **check for pay updates** again.

if no recalculation issues remain, both indicators return to green and **submit for approval** becomes available.

{% hint style="info" %}
#### What happens if P or T is red? The page disables **Submit for Approval** until payroll is recalculated and checked again.
{% endhint %}

### how do I use check for pay updates?

use **check for pay updates** to refresh the payroll review checks before submitting.

1. click **check for pay updates**.
2. wait for the system to complete the check.
3. review the indicator results and any prompts shown.

run this check again if the page has been open for a while before your final review. if P or T is red, review and recalculate the flagged employees before continuing.



***

## pay check adjustment

### how do I use paycheck adjustment?

use **paycheck adjustment** when payroll values need a direct payroll-side correction before approval.

&#x20;this is the correct page for manual payroll adjustments during the masterlist review stage.

**navigation:**\
go to **pay check → pay run → view payroll masterlist → paycheck adjustment**

### what can I do from this page?

this paycheck adjustment supports two different payroll-side correction methods:

* <mark style="color:violet;">**adjustment**</mark> is used for payroll-side workday or pay corrections such as workday, overtime, holiday, night shift differential, leave, absent, tardiness, and undertime directly into the current open pay run
* <mark style="color:violet;">**ingestion**</mark> is used to add payroll-entry amounts into assigned categories such as allowance, other earnings, other deductions, loans, contributions, and withholding tax.  add or off set earning-side entries or deduction-side entries.

in this user guide, “adjustment” is used loosely and may also refer to ingestion.



### how do I create a paycheck adjustment?

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 6.44.40 AM.png" alt=""><figcaption></figcaption></figure>

1. from the payroll **masterlist** , click on the **paycheck adjustment** tab.
2. a new tab/page will open while keeping the main masterlist accessible.
3. in the newly opened page, proceed to add a new paycheck adjustment.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 8.02.18 AM.png" alt=""><figcaption></figcaption></figure>

4. select the employee to whom you want to apply the paycheck adjustment. Selecting an employee name is a required field.&#x20;

{% hint style="info" %}
**select employee   (\*)** - selects the employee receiving the correction.
{% endhint %}

5. choose **pay category**.  determines which payroll-item category the entry belongs to.  choosing a pay category is a required field.   the following pay category options are available:



* **work day**
* **overtime**
* **holiday**
* **nsd**
* **leaves**
* **absent**
* **tardiness**
* **undertime**
* **allowance**
* **other earnings**
* **other deductions**
* **loans**
* **contributions**
* **withholding tax**



<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 5.44.58 AM.png" alt=""><figcaption></figcaption></figure>



6. choose a **pay item**.  Options are listed based on the pay category selected.  Choosing a pay item is a required field.

{% hint style="info" %}
**pay item (\*)** - lists the specific payroll item available under the selected pay category.
{% endhint %}

7. complete remaining **entry fields -** the rest of the row changes based on the selected payroll item.  Some items ask for a date, hours, rate-based value, or a custom amount.  Others use only a smaller set of fields.\
   \
   Common entry field behavior:<br>

* **date (\*)** - records the effective date of the payroll entry. appears when the selected item is date-based (i.e overtime, etc)
* **current and new rate** - shows the current rate or the updated rate context when applicable. appear when the selected item uses rate-based calculation (i.e workday, etc,)
* **rate %** - applies percentage-based logic when supported. appears when the selected item uses percentage-based logic.
* **custom amount** - lets you enter the amount directly when the item supports amount-based entry (i.e. allowance, deminimis)
* **total hours** - used when the entry is hour-based.
* **amount** - records the amount to be saved when the selected item uses direct amount entry or calculated amount output.



8. once done, click **save** to save the current payroll adjustment entry.&#x20;
9. click on **Add more** to add another pay adjustment entry to the same employee or to another employee.
10. **click on View/manage ingestion** to review, edit, or delete a pay adjustment entry.

###

### when to use payroll adjustments?

use the normal payroll modules first when the change belongs to the employee's regular payroll setup.

for example:

* if the employee should receive an earning or deduction through normal setup, create or assign it through the proper module
* if the item can be assigned as a valid one-time payroll entry in the normal module, use that standard assignment flow first
* if the issue is with worked time, attendance, or payable hours, correct it through the timesheet or the proper hours workflow

if the correction can be handled through the standard modules in ashima, use those. these follow the proper rules for taxable and non-taxable reporting and will make it easier for you to manage.

use **payroll adjustment** when a correction needs to be applied directly and urgently (last minute corrections) to the current open pay run.

you can also use this when the amount cannot be added or deducted through the standard earnings or deductions module entries in ashima.

{% hint style="info" %}
as a best practice, avoid relying on **Paycheck Adjustment** for corrections that can be handled through the standard earnings and deductions modules.

use it only as a last resort—for urgent, last-minute corrections that cannot be easily processed through the standard modules.<br>
{% endhint %}

### which adjustment entry should I use for basic pay/workday corrections?

here’s a quick guide to help you choose the right adjustment entry for basic pay or workday corrections:

* **Underpaid:** Missed timesheet / unpaid workday → Use **Work Day (positive)** to add pay
* [**Overpaid**](./#use-case-basic-pay-overpayment)**:** Excess hours or overpaid workday (from previous payroll) → Use **Work Day (negative)** to deduct pay
* **Actual absence (should reduce basic pay)** → Use **Absent (positive)**
* **Actual tardiness (should reduce basic pay)** → Use **Tardiness (positive)**
* **Actual undertime (should reduce basic pay)** → Use **Undertime (positive)**

Use this as a reference when adjusting pay to ensure entries are applied correctly.<br>

{% hint style="info" %}
Use these quick rules first:

* **Work Day** — use to add pay back for a day or hours that should have been paid.
* **Negative Work Day** — use to recover a basic-pay overpayment so the correction stays on the earnings side.
* **Absent** — use to add a missing absence deduction.
* **Tardiness** — use to add a missing tardiness deduction.
* **Undertime** — use to add a missing undertime deduction.
* Use the matching positive deduction entry when the employee should lose pay.
* Do not use **Absent**, **Tardiness**, or **Undertime** when the issue is really a basic-pay overpayment.
{% endhint %}

### use case: basic-pay overpayment

if the employee was overpaid on **basic pay** from previous payroll, keep the correction on the earnings side.

use **work day** with a negative amount when the goal is to:

* take back overpaid basic pay
* bring taxable pay down with the recovery
* let payroll and tax reporting reflect that the overpayment happened on pay, not on attendance deduction

do not force this through **Absent**, **Tardiness**, or **Undertime** if the employee was not actually absent, late, or undertime.



### how do different pay adjustment entries behave?



the exact fields shown on the row depend on the selected **pay category** and **pay item**. Use the table below as a working guide for what each pay-entry group normally requires and how it affects payroll.

<table><thead><tr><th width="109.09375">Pay entry</th><th width="110.1796875">Use case</th><th width="105.6796875">Key fields</th><th width="169.15625">Positive / Negative</th><th width="139.0234375">Tax effect</th><th width="158.34765625">Fix if incorrect entry</th></tr></thead><tbody><tr><td><strong>Work Day</strong></td><td>Pay add-back; basic-pay overpayment recovery</td><td>Date + hours / amount / calculator fields</td><td><p><code>+</code> add pay back; net pay up.</p><p></p><p> <code>-</code> recover  basic pay overpayment; taxable pay down; net pay down</p></td><td>Earnings-side; affects taxable pay and withholding tax</td><td><strong>Edit</strong> values. <strong>Delete and re-add</strong> if wrong item or date</td></tr><tr><td><strong>Overtime</strong></td><td>Overtime pay correction</td><td>Date + hours / rate fields</td><td><p><code>+</code> add overtime pay.</p><p></p><p><code>-</code> reverse overtime pay</p></td><td>Earnings-side; affects taxable pay and withholding tax</td><td><strong>Edit</strong> values. <strong>Delete and re-add</strong> if wrong item or date</td></tr><tr><td><strong>Holiday</strong></td><td>Holiday pay correction</td><td>Date + hours / amount / calculator fields</td><td><p><code>+</code> add holiday pay.</p><p></p><p> <code>-</code> reverse holiday pay</p></td><td>Earnings-side; affects taxable pay and withholding tax</td><td><strong>Edit</strong> values. <strong>Delete and re-add</strong> if wrong item or date</td></tr><tr><td><strong>NSD</strong></td><td>Night shift differential correction</td><td>Date + rate fields</td><td><p><code>+</code> add NSD pay. </p><p></p><p><code>-</code> reverse NSD pay</p></td><td>Earnings-side; affects taxable pay and withholding tax</td><td><strong>Edit</strong> values. <strong>Delete and re-add</strong> if wrong item or date</td></tr><tr><td><strong>Leaves</strong></td><td>Paid leave correction</td><td>Date + hours / amount / calculator fields</td><td><p><code>+</code> add paid leave.</p><p></p><p> <code>-</code> reverse paid leave</p></td><td>Earnings-side; affects taxable pay and withholding tax</td><td><strong>Edit</strong> values. <strong>Delete and re-add</strong> if wrong item or date</td></tr><tr><td><strong>Absent</strong></td><td>Actual absence deduction</td><td>Date +, for some items, <strong>Total Hours</strong> and <strong>Amount</strong></td><td><p><code>+</code> add absence deduction; net pay down.</p><p></p><p> <code>-</code> reduce prior absence adjustment</p></td><td>Deduction-side; not taxable earnings</td><td>Use for real absence only. <strong>Edit</strong> or <strong>Delete and re-add</strong> if wrong</td></tr><tr><td><strong>Tardiness</strong></td><td>Actual tardiness deduction</td><td>Date +, for some items, <strong>Total Hours</strong> and <strong>Amount</strong></td><td><p><code>+</code> add tardiness deduction; net pay down.</p><p></p><p> <code>-</code> reduce prior tardiness adjustment</p></td><td>Deduction-side; not taxable earnings</td><td>Use for real tardiness only. <strong>Edit</strong> or <strong>Delete and re-add</strong> if wrong</td></tr><tr><td><strong>Undertime</strong></td><td>Actual undertime deduction</td><td>Date +, for some items, <strong>Total Hours</strong> and <strong>Amount</strong></td><td><p><code>+</code> add undertime deduction; net pay down. </p><p></p><p><code>-</code> reduce prior undertime adjustment</p></td><td>Deduction-side; not taxable earnings</td><td>Use for real undertime only. <strong>Edit</strong> or <strong>Delete and re-add</strong> if wrong</td></tr><tr><td><strong>Allowance</strong>*</td><td>Allowance correction</td><td> <strong>Amount</strong></td><td><p><code>+</code> add amount.</p><p></p><p> <code>-</code> reverse amount</p></td><td>Depends on allowance type</td><td><strong>Edit</strong> amount. <strong>Delete and re-add</strong> if wrong item</td></tr><tr><td><strong>Other Earnings</strong>*</td><td>Other earning correction</td><td><strong>Amount</strong>  </td><td><p><code>+</code> add amount.</p><p></p><p> <code>-</code> reverse amount</p></td><td>Usually taxable in paycheck flow</td><td><strong>Edit</strong> amount. <strong>Delete and re-add</strong> if wrong item</td></tr><tr><td><strong>Other Deductions</strong>*</td><td>Other deduction correction</td><td><strong>Amount</strong></td><td><p><code>+</code> add deduction; net pay down.</p><p></p><p> <code>-</code> reduce deduction; net pay up</p></td><td>Deduction-side</td><td><strong>Edit</strong> amount. <strong>Delete and re-add</strong> if wrong item</td></tr><tr><td><strong>Loans</strong>*</td><td>Loan deduction correction</td><td><strong>Amount</strong></td><td><p><code>+</code> add deduction; net pay down.</p><p></p><p> <code>-</code> reduce deduction; net pay up</p></td><td>Deduction-side</td><td><strong>Edit</strong> amount. <strong>Delete and re-add</strong> if wrong item</td></tr><tr><td><strong>Contributions</strong>*</td><td>Contribution correction</td><td><strong>Amount</strong></td><td><p><code>+</code> add deduction; net pay down.</p><p></p><p> <code>-</code> reduce deduction; net pay up</p></td><td>Deduction-side</td><td><strong>Edit</strong> amount. <strong>Delete and re-add</strong> if wrong item</td></tr><tr><td><strong>Withholding Tax</strong>*</td><td>Direct tax correction</td><td><strong>Amount</strong> </td><td><p><code>+</code> add tax deduction; net pay down.</p><p></p><p> <code>-</code> reduce tax deduction; net pay up</p></td><td>Direct tax deduction; not the same as adding taxable pay</td><td><strong>Edit</strong> amount. <strong>Delete and re-add</strong> if wrong item</td></tr></tbody></table>

`*` Ingestion entry.   Entries without `*` are adjustment entries.

#### important note about date-based adjustment items.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 5.43.29 AM.png" alt=""><figcaption></figcaption></figure>

date-based entries can require supporting values before they can be saved. for some workday-related entries, the page can require both **total amount** and **total hours**.

if you are working on a date-based correction, review **View/Manage Ingestion** first before adding another entry for the same employee and date.

###

### what happens after I save a payroll adjustment entry?

the page asks you to confirm the save, then stores the payroll entry in the current pay run. &#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 5.44.36 AM.png" alt=""><figcaption></figcaption></figure>

you can review saved entries in **View/Manage Ingestion**

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 5.43.58 AM.png" alt=""><figcaption></figcaption></figure>

edit or delete saved entries if a correction was entered incorrectly

after saving:

* the page resets back to a new blank row
* the saved line can be reviewed in **View/Manage Ingestion**
* the payroll effect should be reviewed again after recalculation

after saving an entry, return to masterlist review and recalculate if the page prompts you to do so.

###

### what happens if I make a mistake on the adjustment&#x20;

if a saved payroll adjsutment entry is wrong edit or delete saved entries that was entered incorrectly:

1. open **View/Manage Ingestion**
2. review whether the payroll item already exists as an active saved line
3. use **Edit** if you want to correct the saved line
4. use **Delete** if you want to remove it completely, then re-add the correct entry

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 1.14.20 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 1.12.29 PM.png" alt=""><figcaption></figcaption></figure>

do not assume saving the same item again will create a second separate correction line.  \
\
please check the [pay entry guide ](./#which-adjustment-entry-should-i-use)to understand the best approach to take when fixing a mistake on the entry.&#x20;



### how do I delete a saved payroll adjustment entry?

delete it from **View/Manage Ingestion**.

a prompt is displayed for you to confirm if you wish to proceed with the deletion:

`Are you sure you want to delete the selected ingestion(s)? This action cannot be undone.`



* delete removes the active payroll correction from the current pay run
* the action should be treated as not undoable from the page

###

### where do payroll adjustments and ingestions appear in employee pay details?

**employee pay details** shows payroll entries under the section they affect.

common display patterns are:

* **adjustment** - earnings-side corrections such as **work day**, **overtime**, **holiday premium**, **night differential**, and **paid leave**
* **ingestion** on the earnings side - paycheck-entry earnings such as **allowance**, **other earnings**, and some payroll-side de minimis results
* **ingestion** on the deductions side - saved deduction entries such as **other deductions**, **loans**, **contributions**, and **withholding tax**
* **absent**, t**ardiness**, and u**ndertime** - shown inside their own deduction breakdowns

#### rules or warnings

* the available **pay item** values depend on the selected **pay category**
* some items require calculator values, not just a direct amount
* do not assume every repeated save creates a second active row
* after saving, editing, or deleting an entry, return to payroll review and recalculate if the page prompts you to do so



***

## payroll exclusion

### how do I use payroll exclusion?

use **payroll exclusion** to review, remove, or reinstate employees for the current payroll output. \
\
employees left in the masterlist at submission will be included in the final payroll.

**navigation:**\
go to **pay check → pay run → view payroll exclusion**

### what does the exclusion page display?

* a searchable listing of excluded employees for the selected payroll set
* the reason recorded for each exclusion or inclusion change
* a **Download** option for the exclusion listing



<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 12.15.31 PM.png" alt=""><figcaption></figcaption></figure>

###

### how do I exclude or include an employee?

1. open the relevant **exclusion** page.
2. click **exclude / include employees**.
3. select the employee in **Employee Name**.
4. set **Exclude** to **Yes** to exclude or **No** to include back.
5. enter **Reason** if needed.
6. click **save**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-27 at 12.15.19 PM.png" alt=""><figcaption></figcaption></figure>

#### Fields

* **employee name (\*)** — selects the employee to update.
* **exclude (\*)** — controls whether the employee is excluded or included.
* **reason** — records why the payroll membership changed.

`(*) Required fields must be completed before saving.`

###

### what happens after I exclude an employee?

the employee is removed from the current payroll output. their payroll is not processed for this run, and the exclusion is recorded with the date and payroll period for audit purposes. \
\
you can include them again before submission if their status changes.

{% hint style="info" %}
common exclusion reasons include no timesheet submission and AWOL.
{% endhint %}

exclusion applies to the current payroll set only. It does not permanently remove the employee from payroll.

### how to re-include an excluded employee

use the same payroll exclusion form to add the employee back to the payroll you are reviewing.

1. open view payroll exclusion for the correct pay run.
2. click exclude / include employees.
3. select the employee in Employee Name.
4. set Exclude to No.
5. enter Reason if needed.
6. click save.<br>

### what happens after I include the employee back?

the employee is no longer treated as excluded for that payroll period and can return to the payroll output for that payroll review.

after including the employee back:

* review the payroll listing again
* recalculate if the page prompts you to do so
* confirm the employee is back in the payroll counts and review pages before approval

after including an employee back, review the payroll listing, recalculate if prompted, and confirm the employee is back in the payroll counts before approval.

{% hint style="info" %}
#### notes

* exclusion applies to the current payroll set. tt does not permanently remove the employee from payroll.
* if the employee is included again later, they return to the current payroll review.
* employees left in the masterlist remain part of the payroll output used for later actions.
{% endhint %}

*



***

## Pay Draft

### what  is a pay draft?

a **pay draft** lets employees view a draft version of their payslip before payroll is closed.

normally, employees can only view their payslip after payroll is closed and payslips are generated/released. the Pay Draft function makes a draft payslip visible earlier - while the pay run is still open - so employees can review current earnings and deductions before payroll is finalized.\
\
the page guidance may also refer to this as a **pay summary draft**.



#### how do I send a pay draft?

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 4.38.32 AM.png" alt=""><figcaption></figcaption></figure>

use **send pay draft** when you want employees to view their draft payslip in the employee portal before payroll is closed.

1. open the relevant payroll masterlist.
2. recalculate the pay run if you have not done so recently.
3. click **send pay draft**.
4. choose to send it to all or to specific employees only.&#x20;

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 4.38.43 AM.png" alt=""><figcaption></figcaption></figure>



make sure the pay run has been recalculated before sending. the page warns that sending without recalculation may result in discrepancies in what employees see. because this action sends a notification to employees, review the payroll state carefully before using it.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-28 at 4.39.03 AM.png" alt=""><figcaption></figcaption></figure>

you can send a pay draft more than once before payroll closes. Each time, the masterlist updates the Last Sent time and Sent Count.

### what happens after you send a pay draft?

* employees will receive an email and can review their pay summary draft (draft payslip).

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 1.49.11 PM.png" alt=""><figcaption></figcaption></figure>



* the masterlist page shows a history line such as **Last Sent** and **Sent Count**.
* companies can send pay draft more than once before payroll closes.

{% hint style="info" %}
#### rules or warnings

* recalculate first before sending a pay draft.
* the page warns that sending a pay draft without recalculation can cause discrepancies.
* treat pay draft as an employee-facing communication step and review it carefully before use.
{% endhint %}



***

## pay run approval

### how do I submit pay run for approval (payroll approval)?

usse **submit for approval** when payroll review is complete and the payroll is ready to move to the approval stage.

**navigation:**\
go to **pay check → pay run → view payroll masterlist**

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 12.45.19 AM.png" alt=""><figcaption></figcaption></figure>

#### steps

1. open the relevant payroll masterlist.
2. review the masterlist table, adjustments, and exclusions.
3. click **check for pay updates** and confirm both P and T indicators are green.
4. click **submit for approval**.
5. **choose which pay group** you want to submit for approval.
6. review the confirmation and proceed.

the confirmation explains that once the pay run is submitted for approval, it is locked and no further changes or updates can be made. it also reminds you to run Check for Pay Updates first, because submitting without recalculation may result in pay discrepancies.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 12.50.28 AM.png" alt=""><figcaption></figcaption></figure>



submit only after payroll values, exclusions, and adjustments are final for the current review cycle.

### what happens after I submit pay run for approval?

when submission is completed:

* the payroll is sent to the configured payroll approver workflow.
* an approval email with a payroll approval link is sent to the approver.
* a payroll approval To Do item is created for the approver.
* the pay run status changes to **Waiting for Approval**.

approvers can review and act on the payroll from the approval email link or from the payroll approval To Do item.

### pay run approval and rejection

once submitted, approvers can review payroll from the approval email link or from the payroll To Do item. if no action is taken, payroll remains in **Waiting for Approval**.

* **if approved** — the pay run becomes **Closed** and moves to closed-payroll actions.
* **if rejected** — the pay run becomes **Rejected** and returns to payroll review for correction and resubmission.

### can approvers approve or reject payroll from email or to do?

yes. the approval workflow supports review from:

* the approval email link
* the payroll approval To Do page

from either view, the approver can review the payroll summary, approve the payroll, or reject it.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 1.00.32 AM.png" alt=""><figcaption></figcaption></figure>

### **how can I check who the pay run approver(s) are?**

Go to **Settings > Workflow > Payroll**.

This page will show the assigned pay run approver(s).

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 2.00.02 PM.png" alt=""><figcaption></figcaption></figure>

### what happens if the payroll is left pending?

If the approver does not act, the payroll remains in **Waiting for Approval**. It does not return to the open draft state on its own.

### what happens when payroll is approved?

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 2.19.19 PM.png" alt=""><figcaption></figcaption></figure>

when final approval is completed:

* the payroll approval status is marked as complete.
* the pay run status changes to **Closed**.
* [the payroll moves into closed-payroll actions:](./#what-can-i-do-on-a-closed-payroll-masterlist) \
  \* download masterlist\
  \* download bank file, \
  \* print payslip \
  \* generate payslip (payslip release)

closed payroll should be treated as final for normal payroll review purposes.

### what happens when payroll is rejected?

when payroll is rejected:

* the pay run status changes to **Rejected**.
* the payroll leaves the approval queue.
* the payroll can return to payroll review so it can be corrected and resubmitted.

review rejected payroll carefully before resubmitting for approval.

###

### what can I do on a closed payroll masterlist?



<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 2.19.11 PM (2).png" alt=""><figcaption></figcaption></figure>

\
after payroll is approved and closed, the masterlist remains available for admin actions. the review-stage buttons (Check for Pay Updates, Send Pay Draft, Submit for Approval) are no longer shown. \
\
in their place, the bottom action area changes to:

* **download** - download the masterlist for the closed payroll
* **download Bank File** - opens the bank file output step
* **print payslip** - opens the payslip print action. The print dropdown offers multiple layouts: **Default**, **By Two / Page**, and **By Four / Page**.
* **generate payslip** - triggers the payslip generation step. A confirmation prompt appears before the system begins generation.

you can still search for a specific employee and review the payroll summary table on a closed masterlist.

### what is the difference between generate payslip and print payslip?

use the payslip area to review how payroll is presented to employees after payroll is closed or released.<br>

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 2.19.25 PM.png" alt=""><figcaption></figcaption></figure>

**generate payslip** starts the payslip generation step after closed payroll.\
\
clicking **generate payslip** starts the payslip generation process after payroll is closed. this means:

* payslips become available in the employee portal for employees to view
* an email notification is sent to employees letting them know their payslips are now available

payslips can only be generated once. after generation, the **generate payslip** button will be disabled (grayed out).

{% hint style="info" %}
**Note:** in Ashima, payslips are not automatically generated or made visible to employees once payroll is approved or closed.

the payroll admin must manually generate the payslips to make them available on the employee portal. this is to ensure payroll admins have completed the necessary fund transfers first before releasing the payslips to employees.
{% endhint %}

**print payslip** opens the printing options for the available payslip layouts. go to [how to print payslip](./#how-to-print-payslips) click here to know more about options on printing.



### how do I download the payroll masterlist?

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 2.25.21 PM.png" alt=""><figcaption></figcaption></figure>

use **download** to export the payroll masterlist from either an open or closed payroll. The exported file name reflects the payroll status so you can distinguish a working review export from a final closed-payroll export.

**navigation:** go to **pay check → pay run → view payroll masterlist**

#### steps

1. open the relevant payroll masterlist.
2. click **download**.
3. <mark style="color:violet;">**step 1: choose your export layout:**</mark>

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 4.58.57 PM.png" alt=""><figcaption></figcaption></figure>

* **Download ALL Columns** - includes all payroll data fields in the export.
* **Download LIMITED Columns** - includes the main payroll columns but removes zero-value fields automatically. Use this for a cleaner export when you only need columns with active values.
* **Download CUSTOM Columns** - lets you manually choose which fields to include.

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 2.25.43 PM.png" alt=""><figcaption></figcaption></figure>



4. <mark style="color:violet;">**step 2: add up to three extra custom employee fields if needed.**</mark>

* the custom field picker lets you add up to three extra employee fields as additional columns. Examples include Department, Payroll Group, Cost Center, Employment Type, Job Position, Location Assigned, Rank, and Report to Name. \
  \
  a search box is available to find fields quickly.

<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 5.10.14 PM.png" alt=""><figcaption></figcaption></figure>



5.  <mark style="color:violet;">**step 3:**</mark> <mark style="color:violet;"></mark><mark style="color:violet;">complete the remaining download options shown by the page.</mark><br>

    the download modal gives three output types:

    * **Download summary** — table listing, fewer columns
    * **Download masterlist** — detailed payroll columns
    * **Download ingestion** — detailed ingestion items only



<figure><img src="../../.gitbook/assets/Screenshot 2026-04-29 at 4.59.21 PM.png" alt=""><figcaption></figcaption></figure>

### what does download ingestion show?

**download ingestion** gives a dedicated ingestion file with one row per saved ingestion item.

the dedicated ingestion download lists these columns:

* **Employee Id**
* **First Name**
* **Last Name**
* **Ingestion Category**
* **Ingestion Item**
* **Tax Rule**
* **Amount**

### where does ingestion appear on the masterlist page itself?

ingestion is not shown as one separate visible column on the live masterlist page.

on the page, its effect is already folded into payroll totals such as:

* taxable pay
* deductions
* withholding tax
* net pay

### how is ingestion reported in the masterlist export?

when **Include Ingestion Breakdown** is set to **Yes**, the masterlist export adds a second row for the employee with **Source = ingestion**.

that extra row maps the ingestion amount into the payroll column it affects, instead of putting every item into one single "ingestion" column.

Examples:

* **Work Day** goes into **Taxable Basic Pay**
* **Tardiness** goes into **Tardiness**
* **Undertime** goes into **Undertime**
* **Absent** goes into **Absent**
* **Leaves** goes into **Leave**
* **Overtime** goes into **Overtime**
* **Holiday** goes into **Holiday** and **Total Holiday & Rest Day**
* **NSD** goes into **Night Shift Differential**
* **SSS**, **PHIC**, **HDMF**, **HDMF I**, **HDMF II**, and **Withholding Tax** go into their matching statutory or tax columns
* dynamic entries such as **Allowance**, **Other Earnings**, **Other Deductions**, and some loan headers are placed into the matching named dynamic columns

this means the ingestion breakdown row is column-mapped, not one single summed narrative line.



## payroll lock

### what should administrators know about locked requests?

once payroll is already **Waiting for approval** or **Closed**, the original pay run should be treated as no longer changeable through normal payroll review.

some payroll-affecting requests may still appear in review or **To Do**, but they can show **Locked for payroll processing** or behave as no longer approvable through the original payroll cycle.

### what happens to requests that come in after payroll is already in approval or closed?

once a pay run is **Waiting for Approval** or **Closed**, it should be treated as no longer changeable through normal payroll review. This applies to:

* admin-initiated payroll-affecting updates
* late employee timesheet, overtime, or leave requests
* late manager approvals for payroll-affecting items

requests submitted after the payroll moved forward can become locked. the portal may show these items with a lock indicator and the note **Locked for Payroll Processing**.

of the payroll is already closed, the request can show that it is connected to a closed payroll and can no longer be approved through the original pay run.

do not approve these requests through the original pay run. See [Post Payroll Adjustments ](./#what-are-post-payroll-adjustments-ppa)below for the correct process.

{% hint style="info" %}
Late requests should not be approved through the original closed or waiting-for-approval payroll. Reapply or reinitiate them through the PPA process when eligible.
{% endhint %}

### what should I do with expired to do items?

some payroll-affecting requests remain visible in **To Do** even after the connected payroll is no longer available for normal approval.

when this happens:

* the item may remain listed for visibility and follow-up but is no longer actionable as a normal open-pay-run approval.
* if the request still shows a pending action, the approver should reject it so it is cleared from the original approval flow.
* if the correction still needs to be processed, re-initiate it through Post Payroll Adjustments instead of approving from the old To Do item.

***

## post payroll adjustments (PPA)

#### what are PPA's?

**post payroll adjustments** are payroll corrections handled after the original pay run has already moved past the normal open review stage.

use PPA when a payroll-affecting update is raised too late for the original open pay run, such as:

* a missing timesheet
* an overtime entry that was not filed in time
* a leave application or time-related correction that affects already-processed payroll

when a late correction is approved through the PPA process, the resulting payroll effect carries into the current open pay run as a post-payroll adjustment. depending on the correction, this carry-over can be either positive or negative.

#### what settings control whether PPA is allowed?

PPA is controlled by company settings. PPA is only available if your company has enabled this function, and only within the allowable past-payroll period set by your company.&#x20;

these settings determine:

* whether **Post Payroll Adjustment** is enabled at all
* whether employees are allowed to start PPA requests
* how far back a closed payroll date can still be handled through PPA

if the company turns off employee-initiated PPA, employees cannot file PPA requests even if PPA remains available for admins.

#### what can PPA cover?

PPA is used for eligible late payroll corrections after the original payroll is already closed and can no longer be updated through the normal open-payroll flow.

**common PPA coverage includes**:

* missing timesheet correction
* timesheet adjustment
* late overtime application
* late leave application
* open-shift PPA
* payroll effects that can later appear as post-payroll adjustments such as workday, tardiness, undertime, leave, overtime, and night shift differential

not every late request is automatically eligible for PPA.  **the following are not allowed through PPA:**

* corrections that fall during a holiday
* shift change adjustments connected to a closed payroll
* items that were already processed as PPA once before

#### how far back can PPA be used?

PPA only works within the company's allowed lookback period.

this setting limits how many past payroll periods can still be corrected through PPA. If a date is already outside that allowed range, the system blocks the request for that period.

if no custom company setting has been saved, the source logic falls back to a default lookback of **6 payroll periods**.

#### when should I use PPA?

Use PPA only when a correction is discovered after payroll has already moved forward and the original pay run can no longer be updated through the normal open-pay-run flow. Do not use PPA for corrections that can still be handled within the original open pay run.

#### how do Post Payroll Adjustments appear in payroll?

PPA items appear in payroll detail and payslip output as separate post-payroll adjustment values rather than as standard open-pay-run entries. This keeps them identifiable as corrections to prior payroll periods.

In some payroll displays and exports, certain PPA categories may appear grouped. For example, **Holiday / Rest Day** may appear together rather than as two completely separate lines.

#### how does PPA affect payroll?

Approved PPA corrections are carried into a later open pay run as post-payroll adjustments.

These adjustments can be:

* positive
* negative

#### who can start a PPA?

PPA can be started by either the employee or the admin, depending on the module and the company settings.



* **Employee-initiated PPA** — the employee files a late correction after the original payroll is closed. This follows the normal approval workflow for that request type and is reviewed in To Do before the payroll effect is carried into a later open pay run.
* **Admin-initiated PPA** — the admin records the correction directly in the admin portal. This appears in history as **admin initiated** and does not require employee-side approval.

#### does employee-initiated PPA require approval?

yes. when the PPA is started by the employee, it follows the normal approval workflow for that request type.

in practice, this means:

* the request is submitted as a PPA request
* approvers review it in **To Do**
* once approved, the payroll effect is carried into a later open pay run

#### does admin-initiated PPA require approval?

no, admin-initiated PPA is recorded directly.   it can appear in history as **admin initiated**. this is used when the admin is applying the correction directly instead of waiting for the employee to file it through the employee portal.



***

## payroll entries

usse the payroll-entry pages to review how earnings, deductions, contributions, withholding tax, and disbursement-related values appear in payroll.

#### how does ashima group pay entries?

ashima groups pay entries based on how they affect payroll.

* [**earnings**](./#earnings) add to the employee's pay. These include items such as allowances, de minimis, 13th month, other earnings, and retroactive pay.
* [**deductions**](pay-items-and-statutory-review/deduction.md) reduce the employee's pay. These include items such as government loans, third party loans, insurance, and other deductions.
* [**contributions**](./#contributions) are statutory or company-managed payroll deductions tied to required contribution types such as **SSS**, **PHIC**, and **HDMF**.
* **withholding tax** is the payroll tax deducted from the employee's pay based on the employee's taxable payroll result and tax setup.
* **disbursements** are payment-side payroll items that are tracked separately from normal earnings and deductions but still form part of the employee's overall payroll output.

in simple terms:

* items that increase pay belong under **Earnings**
* items that reduce pay belong under **Deductions**, **Contributions**, or **Withholding Tax**
* items that release or track payment amounts can also appear under **Disbursements**

this structure helps administrators know where to create a pay item, where to assign it, and how it will appear later in payroll review, masterlist totals, and payslips.

#### what payroll entry groups are part of Paycheck?

**earnings**

* allowances
* de minimis
* 13th month
* other earnings
* retroactive pay

**deductions**

* government loans
* third party loans
* insurance
* other deductions

**contributions**

* SSS
* PHIC
* HDMF
* HDMF I
* HDMF II

**other payroll entries**

* withholding tax
* disbursements

***

## payroll reference | calculation guide

### how is payroll calculated in Ashima

use these formulas to explain how Ashima builds pay. The examples below are simplified so administrators can understand the result they see in payroll review.

### what is the general net pay formula in ashima?

ashima builds payroll in this order:

1. **Regular earnings base**
2. **Taxable pay**
3. **Non-taxable pay**
4. **Gross pay**
5. **Net pay**

use this simple pattern:

<mark style="color:violet;">`Net Pay = Gross Pay - Tax - Contributions - Loans - Other Deductions - Other Payroll Deductions`</mark>

And:

<mark style="color:violet;">`Gross Pay = Taxable Pay + Non-Taxable Pay`</mark>

#### how is net pay calculated for monthly-paid employees?

**for a monthly-paid employee,** the starting point is the employee's cutoff basic pay.

use this simple guide:

<mark style="color:violet;">`Regular Earnings Base = Basic Pay - Absences - Tardiness - Undertime`</mark>

<mark style="color:violet;">`Taxable Pay = Regular Earnings Base + taxable earnings and taxable payroll adjustments`</mark>

<mark style="color:violet;">`Non-Taxable Pay = non-taxable earnings`</mark>

<mark style="color:violet;">`Net Pay = Taxable Pay + Non-Taxable Pay - total deductions`</mark>



**for a semi-monthly monthly-paid employee**, the basic pay usually starts from:

<mark style="color:violet;">`Basic Pay = Monthly Rate / 2`</mark>

for monthly payrolls, ashima uses the full monthly rate. if the employee joins mid-period or has a mid-period salary increase, ashima can replace the flat starting amount with a prorated amount for the covered cutoff.

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

#### how is net pay calculated for hourly-paid employees?

For hourly-paid employees, Ashima starts from payable rendered hours.

Use this simple guide:

<mark style="color:violet;">`Basic Pay = Payable Hours x Hourly Rate`</mark>

<mark style="color:violet;">`Taxable Pay = Rendered Basic Pay + taxable additions - attendance and payroll deductions that apply`</mark>

<mark style="color:violet;">`Net Pay = Taxable Pay + Non-Taxable Pay - total deductions`</mark>

**Example**

* Payable hours: `80`
* Hourly rate: `150`
* Basic pay: `12,000`
* Tardiness deduction: `300`
* Overtime pay: `600`
* Total deductions after tax and contributions: `1,900`

`Taxable Pay = 12,000 - 300 + 600 = 12,300`

`Net Pay = 12,300 - 1,900 = 10,400`

#### how is net pay calculated for daily-paid employees?

For daily-paid employees, Ashima starts from payable rendered days.

Use this simple guide:

<mark style="color:violet;">`Basic Pay = Payable Days x Daily Rate`</mark>

<mark style="color:violet;">`Taxable Pay = Rendered Basic Pay + taxable additions - attendance and payroll deductions that apply`</mark>

<mark style="color:violet;">`Net Pay = Taxable Pay + Non-Taxable Pay - total deductions`</mark>

**Example**

* Payable days: `10`
* Daily rate: `700`
* Basic pay: `7,000`
* Absence deduction: `700`
* Holiday pay: `500`
* Total deductions after tax and contributions: `1,000`

`Taxable Pay = 7,000 - 700 + 500 = 6,800`

`Net Pay = 6,800 - 1,000 = 5,800`

***

### how is salary calculated for a new employee who joins mid-period?

ashima does not give a mid-period joiner the full cutoff pay by default. It builds the employee's pay from the payroll-ready rendered amounts that fall from the hire date through the end of the cutoff.

use this guide:

* **Monthly-paid**: rendered payroll amounts from hire date to cutoff end, based on the employee's schedule and payable time
* **Hourly-paid**: payable hours from hire date onward x hourly rate
* **Daily-paid**: payable days from hire date onward x daily rate

for monthly-paid employees, the practical explanation is:

<mark style="color:violet;">`Prorated Basic Pay = Sum of payroll-ready rendered amounts from hire date to period end`</mark>

ashima builds that amount from the employee's working schedule and payable time in the cutoff.

**Example: monthly-paid new hire**

* Monthly rate: `30,000`
* Daily equivalent used by payroll: `1,000`
* Payable workdays after hire in the cutoff: `6`

`Prorated Basic Pay = 6 x 1,000 = 6,000`

the employee is paid for the payable portion of the cutoff, not the full `15,000` semi-monthly amount.

***

### how is a mid-period salary increase calculated?

when a salary increase takes effect inside the payroll period, Ashima does not simply replace the whole cutoff amount with the new rate. It splits the regular scheduled time before and after the effective date, then prices each part using the matching rate.

use this guide:

* **Monthly-paid**: old equivalent rate for scheduled payable time before effectivity + new equivalent rate for scheduled payable time from effectivity onward
* **Hourly-paid**: payable hours before effectivity x old hourly rate + payable hours from effectivity onward x new hourly rate
* **Daily-paid**: payable days before effectivity x old daily rate + payable days from effectivity onward x new daily rate

this is the clearest simple formula:

<mark style="color:violet;">`Mid-Period Salary = (Old Rate Portion) + (New Rate Portion)`</mark>

Attendance deductions are still applied after that. If the new rate is already effective at the start of the cutoff, Ashima can use the new rate for the whole cutoff instead of splitting it.

**Example: monthly-paid employee**

* Old daily equivalent: `1,000`
* New daily equivalent: `1,200`
* Workdays before increase: `7`
* Workdays from increase date onward: `3`

`Salary for the cutoff = (7 x 1,000) + (3 x 1,200) = 10,600`

***

## payslips

use the payslip area to review how payslip is presented to employees after payroll is closed or released.

this guide covers three pages that work in sequence:

1. **Payslip History** — review the employee's released payroll periods and open a specific payslip.
2. **Payslip Details** — review the full earnings and deductions breakdown for one payslip.
3. **Print Payslip** — open the condensed printable format used for sharing or download.

#### what pages are available in the Payslip area?

| Page                | What it is for                                                                                     |
| ------------------- | -------------------------------------------------------------------------------------------------- |
| **Payslip History** | Shows the employee's available payslips by pay period. Use it to find and open a specific payslip. |
| **Payslip Details** | Shows the full earnings and deductions breakdown for one selected payslip.                         |
| **Print Payslip**   | Shows the condensed printable payslip with totals. Used for sharing or download.                   |

#### before you begin: key payslip terms

* **Regular Hours** — the main salary or worked-time earning for the payslip period. This is where basic pay, attendance deductions, and the core payroll result sit.
* **Adjustments** - payroll corrections added directly to the pay run through Paycheck Adjustment.
* **Ingestion** - payroll entries added through the paycheck-entry flow and grouped separately on the detailed payslip view.
* **Post Payroll Adjustment (PPA)** — a late correction applied after the original payroll was already closed.
* **Net Pay** — the final take-home amount after all earnings, deductions, contributions, and tax are applied.

#### what should administrators know about how payslip items are grouped?

ashima groups payroll items by category - not by the order they were saved or entered. The payslip is not a flat list of every saved entry.

the detailed payslip organises items into four layers:

1. **Main payroll earnings** — the regular payroll result for the period, including basic pay and attendance-based changes
2. **Payroll corrections** — items added after the original payroll calculation, such as PPA, Adjustments, and Ingestion entries
3. **Deductions** — statutory deductions, contributions, loans, insurance, and other deductions
4. **Net Pay** — the final payroll result

this means a saved payroll item may appear:

* as its own top-level section
* as a child line inside a larger section
* inside the payroll bucket it affects

for example, a normal allowance assignment appears under **Allowance**. A paycheck-entry allowance correction can appear under **Adjustments** or **Ingestion** depending on how it was added. An absence correction can appear under **Other Adjustments** rather than under **Regular Hours**.

if a saved entry is not where you expect it, check the payroll category it belongs to - not just the name it was saved under.

***

### payslip history

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 3.09.18 PM.png" alt=""><figcaption></figcaption></figure>



use **Payslip History** to review the employee's available payslips and open one for detailed review.

**Navigation:** Go to **Pay Check → \[pay run] → \[employee] → Payslip History**

#### what does this page display?

The page shows the released or available payslips for the selected employee. Each row shows:

* payroll date
* covered payroll period
* link to open the detailed payslip view
* link to open the printable payslip

#### what can I do from this page?

* find and open a specific payslip period in **Payslip Details**
* open the printable payslip format directly
* review older payroll periods for the same employee
* download all payslips for an employee

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 3.14.06 PM.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
This page allows admins to download all payslips for an employee before marking them as end of employment. This ensures a copy is saved to the admin’s computer for any future reference or requirements.
{% endhint %}

####

***

### payslip details

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 3.19.39 PM.png" alt=""><figcaption></figcaption></figure>

use **payslip details** when you need the full breakdown of how the employee's pay was built for one payroll period.

**navigation:** Go to **Pay Check → \[pay run] → \[employee] → Payslip History → \[payslip]**

#### what does this page display?

at the top, the page shows a summary card area with:

* **Payroll Period**
* **Pay Date**
* **Basic Pay**
* **Hourly Rate** (shown for hourly-paid employees)
* **Net Pay**

below the summary cards, the page divides into **earnings** and **deductions**. each section can expand into more detailed rows.

***

### what appears under payslip earnings?

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 3.09.49 PM.png" alt=""><figcaption></figcaption></figure>

depending on the employee's payroll result, the detailed payslip can show these earnings sections:

| Section                           | What it contains                                                               |
| --------------------------------- | ------------------------------------------------------------------------------ |
| **Regular Hours**                 | The main payroll earning block — basic pay, absences, tardiness, and undertime |
| **Paid Leave**                    | Leave pay for the period                                                       |
| **Leave Conversion**              | Leave converted to cash where applicable                                       |
| **Overtime**                      | Overtime pay for the period                                                    |
| **Rest Day / Holiday**            | Rest day or holiday premium pay                                                |
| **Night Shift Differential**      | NSD pay for the period                                                         |
| **Post Payroll Adjustment**       | PPA corrections from prior closed payrolls                                     |
| **Retroactive Pay**               | Prior pay differences carried into this run                                    |
| **Adjustments**                   | Payroll corrections added through Paycheck Adjustment                          |
| **Allowance**                     | Allowance assignments                                                          |
| **De Minimis**                    | De minimis benefit amounts                                                     |
| **Service Charge**                | Service charge earnings                                                        |
| **Hazard Pay**                    | Hazard pay amounts                                                             |
| **Other Earnings**                | Other earning assignments                                                      |
| **Withholding Tax (Adjustments)** | Direct withholding tax corrections                                             |
| **Ingestion**                     | Paycheck-entry earnings grouped together                                       |

not every section appears on every payslip. sections only appear when the employee has a value for that category in the current payroll period.

***

#### how is regular hours broken down?

**Regular Hours** is the main payroll earning block. It can expand into:

* **Hours worked** — the base earning for the period
* **Absences** — attendance deductions for absent days or hours
* **Tardiness** — deductions for late arrivals
* **Undertime** — deductions for early departures

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 3.47.55 PM.png" alt=""><figcaption></figcaption></figure>

this section shows how the employee's core pay for the period was built before other earnings or corrections are applied. Review this section first when the net pay result looks different from what was expected.\
\
it is important to note that [monthly-paid employees ](./#monthly-paid-vs-hourly-paid-payslips)use a different calculation formula compared to hourly-paid employees.

***

#### how are payroll corrections shown under earnings?

ashima separates three kinds of payroll corrections so you can trace where each amount came from.

**post payroll adjustment** covers corrections from prior closed payrolls. It can include:

* Workday, Tardiness, Undertime, Leave, Overtime, Holiday, Night Shift Differential

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 4.03.03 PM.png" alt=""><figcaption></figcaption></figure>

**adjustments** covers corrections added to the current pay run through Paycheck Adjustment. It can include:

* Workday, Overtime, Holiday Premium, Night Shift Differential, Paid Leave, Allowance, Advance Payment, De Minimis, Service Charge, Hazard Pay, Other Earnings

**ingestion** covers payroll entries added through the paycheck-entry flow. It appears as its own grouped section in the detailed payslip when entries were added that way.

the reason for the separation: a normal earned allowance and a paycheck-entry allowance correction are different things even though they both affect allowance pay. keeping them in separate sections makes it easier to trace the source of each amount.

***

### What appears under payslip deductions?

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-03 at 3.10.01 PM.png" alt=""><figcaption></figcaption></figure>



Depending on the payroll result, the detailed payslip can show these deduction sections:

| Section                     | What it contains                                |
| --------------------------- | ----------------------------------------------- |
| **Withholding Tax**         | Normal payroll-calculated withholding tax       |
| **Withholding Tax (Fixed)** | Fixed withholding tax where that method applies |
| **SSS**                     | SSS contribution deduction                      |
| **PhilHealth**              | PhilHealth contribution deduction               |
| **HDMF**                    | Regular HDMF contribution                       |
| **HDMF I**                  | HDMF voluntary contribution                     |
| **HDMF II**                 | HDMF modified contribution                      |
| **HDMF MP2**                | HDMF MP2 savings contribution                   |
| **Insurance**               | Insurance deduction assignments                 |
| **Loans**                   | Government and third-party loan deductions      |
| **Other Deductions**        | Company-defined other deductions                |
| **Other Adjustments**       | Deduction-side payroll corrections              |
| **Ingestion**               | Paycheck-entry deductions grouped together      |

***

#### How are deduction corrections shown?

The payslip separates normal deductions from deduction-side corrections.

**Other Adjustments** covers deduction corrections added to the pay run. It can include:

* Absences, Tardiness, Undertime, Third-Party Loans, Government Loans, Other Deductions

This makes it easier to distinguish what was a normal payroll deduction result from what was a correction added directly to the pay run.

***

#### What can I do from this page?

* Review the full earnings and deductions breakdown for the period
* Expand sections to see date-based or entry-based detail rows
* Trace whether an amount came from the main payroll result, a PPA, an Adjustment, or Ingestion
* Open the printable payslip



***



### How to Print Payslips

Use **Print Payslip** when you need the cleaner condensed format for sharing or download.

**Navigation:** Go to **Pay Check → \[pay run] → \[employee] → Payslip History → \[payslip] → Print**

#### What does this page display?

The printable payslip shows:

* company details
* employee name and employee ID
* job position, department, and location
* payroll date and payroll period
* **Basic Pay**
* **Earnings** with total
* **Deductions** with total
* **Net Pay**

#### How is the printable payslip different from Payslip Details?

The printable payslip is more condensed. It shows the same payroll result but groups some items under larger parent labels such as **regular hours**, **Post Payroll Adjustments**, and **Adjustment** rather than showing every category with the same expanded structure as the detailed page.

Use **Payslip Details** when you need to trace a specific amount or review the full breakdown. Use **Print Payslip** when you need a clean shareable format.



***

### Monthly-Paid vs Hourly-Paid Payslips

#### What is the difference between a monthly-paid and an hourly-paid payslip?

The biggest difference is how **Regular Hours** and **Basic Pay** are interpreted. The structure of the payslip is the same — the reading changes based on the employee's pay type.

***

#### Monthly-paid employees

For a monthly-paid employee, the payslip's main earning block starts from the employee's payroll-period basic pay based on their monthly salary setup.

The monthly-paid payslip reads as:

* payroll-period basic pay for the cutoff
* less Absences
* less Tardiness
* less Undertime
* with other earnings and corrections shown in their own sections

The focus is on how attendance deductions and payroll corrections changed the salary result. The base amount is salary-first — not hours-first.

**Simple example:** An employee on a monthly salary of 30,000 on a semi-monthly payroll starts with a basic pay of 15,000 for the cutoff. If they had 1 day of absence and 2 hours of tardiness, those amounts reduce the regular hours result. Overtime, allowances, or adjustments then appear in their own sections above or below.

***

#### Hourly-paid employees

For an hourly-paid employee, the payslip is more directly tied to payable worked hours and the employee's hourly rate. The **Hourly Rate** field in the summary cards becomes more important when reviewing hourly-paid payroll.

The hourly-paid payslip reads as:

* worked hours for the period
* multiplied by the employee's hourly rate
* reduced by any Tardiness or Undertime
* with other earnings and corrections shown in their own sections

The focus is on hours worked and worked-time adjustments.

**Simple example:** An employee at 150/hour with 80 payable hours starts with a basic pay of 12,000. Tardiness reduces that amount. Overtime adds to it. Other corrections appear in their own sections.

***

### How does paid leave differ between pay types?

For hourly-paid employees, paid leave is treated as a separate earning amount tied to payable hours and is more clearly visible as its own earning line.

For monthly-paid employees, paid leave still appears separately when relevant, but the regular salary view is more salary-based — the payslip does not always show the leave as a distinct hours-based line in the same way.

***

#### What changes in the Basic Pay summary card?

| Pay type         | What Basic Pay shows                                                         |
| ---------------- | ---------------------------------------------------------------------------- |
| **Monthly-paid** | The payroll-period share of the monthly salary — salary-based for the cutoff |
| **Hourly-paid**  | The payable hours multiplied by the hourly rate — hours-first                |

***

### Payslip Review Reference

#### What should administrators check first when reviewing a payslip?

Review in this order:

1. **Payroll Period**, **Pay Date**, and **Net Pay** — confirm you are looking at the right period and the right employee
2. **Basic Pay** — confirm the starting pay value is correct for the employee's pay type
3. **Regular Hours** — review the core payroll earning and any attendance deductions (Absences, Tardiness, Undertime)
4. **Additional earnings** — review Overtime, Rest Day/Holiday, Night Shift Differential, and Allowance
5. **Payroll corrections** — review PPA, Adjustments, and Ingestion entries
6. **Deductions** — review Withholding Tax, SSS, PhilHealth, HDMF, Loans, and Other Deductions

Following this order makes it easier to identify whether a payroll result changed because of the core pay calculation, attendance, an additional earning, a payroll correction, or a deduction.

***



#### Where do payroll adjustments and ingestions appear on the payslip?

The payslip shows each payroll entry under the earnings, deductions, contribution, or tax section it belongs to.

Typical display behavior is:

* **Work Day**, **Overtime**, **Holiday**, **NSD**, and **Paid Leave** corrections appear under the **Adjustment** earnings section
* **Allowance** and **Other Earnings** paycheck entries appear under the **Ingestion** earnings section
* **De Minimis** appears in the de minimis or non-taxable earnings area, with excess handled separately when applicable
* **Other Deductions**, **Loans**, **Contributions**, and **Withholding Tax** paycheck entries appear under the deductions or tax side
* **Withholding Tax (Adjustments)** appears as its own tax-adjustment line
* **Absent**, **Tardiness**, and **Undertime** stay on the deduction side

####

***
