# Shifts

The **Shift** module is where administrators set up work schedules, assign those schedules to employees, and maintain the company holiday calendar used in timekeeping and payroll review.

This module covers three areas that work in sequence:

1. **Shift Planning** — create and maintain the shift types that define how schedules behave.
2. **Shifts Calendar** — review schedules in calendar view by month, week, four-week, or daily layout.
3. **Shifts Overview** — assign shift types to employees, manage rest days, and export or import schedule data.
4. **Holiday Schedule** — maintain the company holiday calendar that affects how schedules and attendance are interpreted.

Build shift types in Shift Planning first. Once a type is ready, assign it from Shifts Overview. Keep the holiday calendar current so schedule and payroll interpretation is accurate.

***

### What pages are available in the Shift module?

The main pages in the Shift module are:\
\
**Shifts Calendar** - the visual calendar view used to review schedules by **Month**, **Week**, **4 Week**, or **Daily** layout.

**Assignment workspace (Shifts)**

* **Shifts Overview** — the weekly employee schedule grid, used to review, assign, remove, download, and import shift assignments.
* **Employee Calendar** — the individual employee schedule view, showing a four-week calendar with shift, holiday, and leave context.

**Holiday Schedule** - for reviewing, adding, updating, deleting, downloading, and importing company holidays.

The shift setup pages used by this module are under **Settings → Shifts**:\
\
**Shift setup (Settings → Shifts)**

* **Regular Shift Template** — for standard fixed workdays and fixed time ranges.
* **Compressed Shift Template** — for employees working longer hours across fewer workdays.
* **Night Shift Template** — for scheduled night-coverage work.
* **Rest Day Shift Template** — for reusable non-working schedule patterns.
* **Flexi Time Shift Template** — for required-hours schedules with flexible start and end times.
* **Open Shift Template** — for schedules with no fixed daily clock-in and clock-out pattern.

**Manage Shifts** — for maintaining, archiving, and restoring created shift templates.

**Import Shifts / Import Flexi Time Schedule** — for bulk-loading shift templates via CSV.

***

### Before you begin: key shift concepts

Review these terms before working in the Shift module.

* **Shift Type** — the schedule template that defines how a schedule behaves: workdays, time ranges, break rules, tardiness handling, and holiday behavior. Created in Shift Planning. Assigned from Shifts Overview.
* **Shift Assignment** — the date-specific schedule applied to an employee. When a date-specific assignment is removed, the employee falls back to their default work schedule from their payroll group.
* **Default Work Schedule** — the base schedule set at the payroll group level. It applies on any date where no date-specific shift assignment exists.
* **Mark as Rest Day** — a shift assignment state that designates selected dates as non-working days without removing the employee from the schedule plan.
* **Archive** — moves a shift template out of the active list without permanently deleting it. Archived templates can be restored. Use archive instead of deletion when the schedule may be needed again later.

***

### What should administrators know about Shift settings?

Use **Settings → Shifts** to define the schedule templates that employees can be assigned to. Use the linked shift-rule pages when you need to control how those schedules behave in approval, attendance interpretation, and payroll.

In practice:

* **Work Schedule Settings** creates the templates that appear in **Shifts Overview** during shift assignment.
* **Night Differential Settings** defines the NSD time window and enabled NSD calculation rules.
* **Holiday Pay Settings** defines whether holiday-related pay needs approval and whether absence-before-holiday rules are enforced.
* **Rest Day Settings** defines whether rest day work is auto-paid or must first go through approval.
* **Schedule Request Settings** defines the lead-time rule for employee schedule-change requests.

Create the schedule template first. Then review the linked rule pages before assigning shifts at scale, especially if your company uses flexi time, open shifts, holiday approval, or rest day approval.

## Shift Planning — Create Shift Types

**Navigation:** Go to **Settings → Shifts**

### Why create shift types before assigning shifts?

Shift types are created first so you can assign a consistent schedule pattern instead of rebuilding the same rules for each employee. Once a shift type is saved, it becomes available for assignment from Shifts Overview and can be reused across any number of employees and date ranges.

Creating shift types in advance also ensures that timekeeping interprets attendance correctly. Break settings, tardiness rules, and holiday behavior are all part of the shift type — they are not set at the time of assignment.

***

### What shift types can administrators create?

**Navigation:** Go to **Settings → Shifts**

| Shift Type     | Use when                                                                           |
| -------------- | ---------------------------------------------------------------------------------- |
| **Regular**    | Employees follow a fixed daily schedule on planned workdays.                       |
| **Compressed** | Employees render longer daily hours across fewer workdays.                         |
| **Night**      | The schedule is intended for night-coverage operations.                            |
| **Rest Day**   | You need a reusable non-working pattern in schedule setup.                         |
| **Flexi Time** | The employee must complete required hours but can work with more time flexibility. |
| **Open Shift** | The schedule should not depend on a fixed daily clock-in and clock-out pattern.    |

The settings pages are not all built the same way:

* **Regular**, **Compressed**, **Night**, and **Rest Day** show weekday-by-weekday schedule templates with **Shift Threshold** and **Tardiness Rule** columns.
* **Flexi Time** shows flexible-hour templates with weekly required hours and login-related rules.
* **Open Shift** shows a simpler template list with **Timekeep Normally On Holiday** behavior.
* **Manage Shifts** is the combined maintenance page for created templates.

\
\
When choosing a shift type, select the one that best matches how attendance should be interpreted — not just how the shift sounds operationally.

***

### How do I create a shift type?

**Navigation:** Go to **Settings → Shifts**, then open the shift type you want to create.

#### Steps

1. Go to **Settings → Shifts**.
2. Open the shift type you want to create — Regular, Compressed, Night, Rest Day, Flexi Time, or Open Shift.
3. Click the action to add a new shift template.
4. Enter the shift details. The exact fields vary by shift type, but the sections below cover what to expect.
5. Review the work pattern, breaks, and schedule rules carefully before saving.
6. Save the template.

#### Fields

The exact fields and layout vary by shift type. These are the common schedule settings across all types:

* **Shift Name (\*)** — the name shown when selecting the shift during assignment. Use a name that is clear enough for other admins to recognise during bulk assignment.
* **Shift Template / Shift Type (\*)** — determines the schedule pattern being created.
* **Workdays / Rest Days** — defines which days are treated as working or non-working.
* **Start / End Time** — defines the planned daily time range for fixed schedules.
* **Required Hours / Total Hours** — defines the expected work duration.
* **Break Settings** — defines lunch break and additional break behavior. Break fields in timesheet logs are enabled or disabled based on this setting.
* **Grace Period / Tardiness Rule** — defines how lateness is handled during timesheet interpretation.
* **Holiday Behavior** — defines how the schedule behaves when the workday overlaps a holiday.

`(*) Required fields must be completed before saving.`

Build the template based on how the shift should be interpreted in timekeeping, not just how it sounds operationally. Review workdays, break rules, and tardiness handling carefully — these settings directly affect timesheet output.

#### Image Placeholder

\[Image: Shift Planning page showing the shift template form with identity, work pattern, time rules, break rules, and attendance rule sections]

***

### What happens after saving?

The shift template becomes available for assignment from **Shifts Overview**.

#### Rules and behavior notes

* Build the shift type based on how attendance should be interpreted, not just how the schedule is labeled operationally.
* Review workdays, break rules, and tardiness handling carefully before saving because these settings affect timesheet interpretation later.
* The exact field order and helper text vary by shift type.

#### Linked settings that affect later payroll behavior

* **Night Differential Settings** defines the NSD time window and enabled NSD calculation rules that can later be assigned in employee compensation.
* **Holiday Pay Settings** defines whether holiday-related pay needs approval and whether absence-before-holiday rules are enforced.
* **Rest Day Settings** defines whether rest day work must be approved before payment.
* **Schedule Request Settings** defines whether employees must submit schedule changes a set number of days in advance.

#### Image Placeholder

\[Image: Shift Planning page showing the shift template form with work pattern, time rules, break rules, and holiday behavior sections]

### Shifts Calendar

Use **Shifts Calendar** when you need a wider visual schedule view before drilling into weekly assignment work.

**Navigation:** Go to **Shifts → Shifts Calendar**

#### What does the Shifts Calendar page display?

The page shows employee schedules in calendar layout instead of a weekly grid.

The live page includes:

* a work-schedule selector
* view options for **Month**, **Week**, **4 Week**, and **Daily**
* previous and next navigation
* schedule cells that can show shift code, time range, and **Rest Day**

#### When should I use Shifts Calendar instead of Shifts Overview?

Use **Shifts Calendar** when you want to:

* scan schedules visually across a larger date span
* compare schedule patterns across teams or dates
* switch quickly between month, week, four-week, and daily views

Use **Shifts Overview** when you need to assign, delete, import, or export schedules.

#### Rules and behavior notes

* **Shifts Calendar** is a review page first.
* The detailed assignment workflow is handled from **Shifts Overview**.
* The page can display the currently selected work schedule together with schedule counts in the calendar cells.

#### Image Placeholder

\[Image: Shifts Calendar page showing the month view, view switcher, work-schedule selector, and schedule cells]

### How do I import shift templates in bulk?

Use the import pages when you need to create multiple shift templates at once instead of entering each one manually.

**Navigation:** Go to **Settings → Shifts → Import**

Two import pages are available:

* **Import Shifts** — for standard shift-template imports.
* **Import Flexi Time Schedule** — for flexible schedule imports.

#### Steps

1. Go to the appropriate import page under **Settings → Shifts**.
2. Click **Download Template** to get the current template for that shift type.
3. Review the required fields and formatting notes shown on the page.
4. Prepare your CSV using the latest template. Upload CSV files only.
5. Upload the file.
6. Review any warning or confirmation prompt before completing the import.

Always use the template for the specific shift type you are importing. Do not reuse templates across shift types.

#### Rules and behavior notes

* Upload CSV files only.
* Use the template for the specific shift type you are importing.
* Do not reuse old templates when the page provides a current one.

***

### Manage Shifts

**Manage Shifts** is used to maintain existing shift templates after they are created. Use it to search for a template, archive templates that should no longer be assigned, and restore archived templates when needed.

**Navigation:** Go to **Settings → Shifts → Manage Shifts**

#### What does Manage Shifts display?

This page lets you:

* review existing shift templates
* search for a specific template
* archive templates that should no longer be assigned
* open **Archived Shifts** and restore templates when needed

#### How do I archive a shift template?

Use **Archive** when a shift template should no longer be available for new assignments but may still be needed later. Archive is the safer maintenance option — it retires the schedule without removing its setup history.

1. Go to **Settings → Shifts → Manage Shifts**.
2. Search for the shift template you want to retire.
3. Use the archive action on that template.

Archived templates move out of the active list and can be reviewed under **Archived Shifts**.

#### How do I restore an archived shift template?

1. Go to **Settings → Shifts → Manage Shifts**.
2. Open **Archived Shifts**.
3. Find the template you want to restore.
4. Use the restore or unarchive action to return it to the active list.

#### How do I delete a shift template?

Use deletion when the shift should no longer remain available as a template and should not stay in the active settings list. Deletion is permanent — use archive instead if there is any chance the template may be needed again.

1. Go to the shift settings page for the shift type you want to maintain.
2. Select the shift template you want to remove.
3. Run the delete action.
4. Review any dependency warning shown before confirming.

**Important:** A shift template cannot be deleted when it is still assigned to one or more payroll groups. The page shows a dependency warning listing the affected payroll groups. Resolve those assignments before attempting deletion.

#### What happens after archive, restore, or delete?

* **Archive** removes the template from the active list without permanently removing it.
* **Restore** returns the template to the active list.
* **Delete** removes the template from the active settings list when deletion is allowed.

#### Rules and behavior notes

* Use **Archive** when the template may still be needed later.
* A shift template cannot be deleted while it is still assigned to one or more payroll groups.
* When deletion is blocked, the page shows the affected payroll-group dependency.

####

***

## Shifts Overview — Assign and Manage Schedules

### Shifts Overview

The **Shifts Overview** page is the employee assignment workspace. Use it to review which shifts are currently assigned to employees, make assignment changes, manage rest days, and export or import schedule data.

**Navigation:** Go to **Shifts → Shifts Overview**

#### What does the Shifts Overview page display?

The page shows a weekly grid with one row per employee and one column per day of the selected week.

Each cell in the grid shows:

* The assigned shift code and scheduled time range
* Break and short break values
* **Total Hours** for that day
* **Rest Day** when no working shift is assigned for that date

The rightmost column shows **Weekly Scheduled Hours** for each employee.

This grid is the main surface for checking assigned shifts, rest days, and weekly hours before making changes.

#### How do I navigate the weekly view?

1. Go to **Shifts → Shifts Overview**.
2. Use **Search** to narrow the list to a specific employee if needed.
3. Review the week shown next to the date field.
4. Use the previous and next arrow buttons to move across weeks.
5. Click **Today** to return to the current week.

#### Fields

* **Search** — filters the overview by employee name.
* **Date** — sets the week displayed in the overview grid. Change this to review a different week.

Review both the daily schedule cells and the **Weekly Scheduled Hours** column before making any assignment changes.

#### How do I review a different week?

1. Go to **Shifts → Shifts Overview**.
2. Use **Search** if you need to find a specific employee.
3. Review the week shown next to the date field.
4. Use the previous and next arrows to move across weeks.
5. Click **Today** to return to the current week.

***

### How do I assign shifts?

Use **Assign Shifts** after selecting one or more employees from the weekly overview. This opens the assignment modal where you choose the shift, date range, and employee scope.

**Navigation:** Go to **Shifts → Shifts Overview**

#### Steps

1. Go to **Shifts → Shifts Overview**.
2. Select the checkbox for one or more employees.
3. Click **Assign Shifts**.
4. In **Work Schedule**, choose the shift type to assign.
5. Set the **From** and **To** dates for the assignment range.
6. In **Select Employees**, choose **Payroll Group** or **Employee** to define the assignment scope.
7. Review the **Employee List** that will be affected.
8. Turn on **Notify Employee** if the employee should receive a notification of the change.
9. Click **Save**.

#### Fields

* **Work Schedule (\*)** — selects the shift type to assign. Choose from the created shift templates available in your company.
* **From (\*)** — sets the start date of the assignment range. Standard bulk assignments are limited to a maximum 90-day range from the start date. Calendar-based assignments support up to a 9-month range.
* **To (\*)** — sets the end date of the assignment range.
* **Select Employees** — defines the assignment scope. Choose **Payroll Group** to assign by group, or **Employee** to assign to individually selected employees.
* **Notify Employee** — sends a notification to the employee when enabled. Use this only when the employee should be informed of the change immediately.

`(*) Required fields must be completed before saving.`

#### What does Mark as Rest Day do?

**Mark as Rest Day** assigns the selected dates as non-working days instead of a working schedule. Use this when the employee should remain part of the schedule plan for those dates but without a working shift. It is available within the same assignment modal.

Use **Mark as Rest Day** when selected dates should be treated as non-working days instead of a working schedule. This is part of the same assignment flow.

#### What happens after I save?

* The system validates the selected dates before applying the assignment.
* If no blocking issues are found, the shifts are assigned immediately.
* For multi-employee assignments, if some employees have conflicts, the page may show a continue step so you can review which items are affected before proceeding. Valid items can be saved while blocked ones are skipped.

Review the selected week before assigning to avoid saving over an existing schedule by mistake.

#### Image Placeholder

\[Image: Edit Employee Shifts modal showing the Work Schedule field, date range, Select Employees mode, Notify Employee toggle, and Mark as Rest Day button]

***

### What can block a shift assignment?

The system checks for conflicts before applying a shift change. Warnings or a continue step may appear when the selected date range includes:

* An ongoing shift — the employee has not yet clocked out and the post-clock-out wait period has not passed.
* A pending timesheet for the selected date — pending timesheets must be approved or rejected first.
* A pending shift request that conflicts with the selected date.
* A pending or approved leave that overlaps the selected dates.
* A date that belongs to a closed pay run — closed pay run dates cannot be changed from the Shift module.

For single-employee updates, the system can show specific warning text explaining what needs to be resolved before the change can be saved. For multi-employee updates, the page can let you continue with valid items while excluding the blocked ones.

If the issue is tied to a closed pay run or another hard conflict, resolve that issue before trying again.

***

### When should I change an employee's shift?

Change an employee's shift when the assigned schedule needs to be corrected or updated for the affected dates. Common reasons include:

* The employee was scheduled under the wrong shift type.
* The employee needs to move to a different planned schedule.
* Selected dates should become rest days.
* An existing custom shift assignment should be replaced with another schedule.

Admin shift changes are applied directly in the portal. Unlike employee shift-change requests, they do not go through an approval workflow.

Before saving, confirm:

* The selected **Work Schedule** is the correct shift type.
* The **From** and **To** dates match the period that should change.
* The selected employee list is correct.
* No closed pay run dates or pending timesheets are in the selected range.

***

### Can I remove an assigned shifts?

Use **Delete** after selecting one or more employees from the weekly overview to remove their date-specific shift assignments.

**Navigation:** Go to **Shifts → Shifts Overview**

#### Steps

1. Go to **Shifts → Shifts Overview**.
2. Select the checkbox for one or more employees.
3. Click **Delete**.
4. Review any warnings or blocking messages shown by the system.
5. Continue only for the items that are safe to remove.

#### What happens when a shift assignment is removed?

Removing a date-specific shift assignment does not leave the employee without a schedule. The system falls back to the employee's default work schedule — set at the payroll group level — for any date where no date-specific assignment exists.

The system applies the same conflict checks used during assignment. Some items in a multi-employee selection may be blocked while others can still be removed.

#### Image Placeholder

\[Image: Shifts Overview bottom action bar showing selected employee count and the Delete action]

***

### How do I download shift assignments?

**Navigation:** Go to **Shifts → Shifts Overview**

#### Steps

1. Go to **Shifts → Shifts Overview**.
2. Click the download button in the bottom action bar.
3. Choose your export type:
   * **XLS** — downloads the currently displayed week in XLS format.
   * **CSV** — downloads the currently displayed week in CSV format.
   * **Custom** — opens the custom download modal for a defined date range or filtered export.

Use XLS or CSV for a quick export of the current week. Use Custom when you need to export a different date range or a specific employee or payroll group.

#### How do I use Custom Download?

1. Click **Download** and choose **Custom**.
2. In **Download By**, choose **All Employees**, **Payroll Group**, or **Employee**.
3. Set the **From** and **To** dates.
4. Choose the **File Type**: XLS or CSV.
5. Click **Check** to validate the request.
6. Once validation passes, click **Download**.

**Download** stays unavailable until the check passes. If the dataset is too large, the page asks you to reduce the date range or narrow the employee selection before retrying.

#### Fields

* **Download By (\*)** — sets the export scope: All Employees, one Payroll Group, or one Employee.
* **From (\*)** — sets the start date of the custom export.
* **To (\*)** — sets the end date of the custom export.
* **File Type (\*)** — selects XLS or CSV.

`(*) Required fields must be completed before the check can run.`

#### Image Placeholder

\[Image: Custom Download modal showing Download By, From, To, File Type, Check button, and Download button]

***

### How do I import shift assignments in bulk?

Use **Import File** when you need to assign schedules to multiple employees at once from a CSV template.

**Navigation:** Go to **Shifts → Shifts Overview → Import File**

#### Steps

1. Go to **Shifts → Shifts Overview**.
2. Click **Import File**.
3. In **Step 1**, click **Download Template** to get the latest CSV template.
4. In **Step 2**, review the column header guide shown on the page.
5. Prepare your CSV using the required format and column headers.
6. In **Step 3**, upload the CSV file.
7. Wait for the import to finish and review the results shown on screen.

#### What does the import require?

The required column headers are:

* **Employee Number / ID Number**
* **Valid From**
* **Valid Until**
* **Schedule Name** — use a valid work schedule name or **Mark as Rest Day**

### Fields

* **Search** — filters the overview by employee name.
* **Date** — changes the week shown in the grid.
* **Today** — returns the page to the current week.
* **Work Schedule (\*)** — selects the shift template to assign.
* **From (\*)** — sets the start date of the assignment or custom download range.
* **To (\*)** — sets the end date of the assignment or custom download range.
* **Select Employees** — lets you assign by **Payroll Group** or **Employee** scope.
* **Employee List** — shows the employees included in the current assignment action.
* **Notify Employee** — sends an employee notification when enabled.
* **Download By (\*)** — sets the export scope for custom download.
* **File Type (\*)** — selects **XLS** or **CSV** for custom download.
* **Upload File (\*)** — uploads the CSV used for shift assignment import.

`(*) Required fields must be completed before saving, checking, or uploading.`

Upload CSV files only. Always download a fresh template before preparing the file — do not reuse old templates. The import may pause on warning or confirmation prompts before the file is fully applied.

#### What happens after saving, deleting, downloading, or importing?

* A valid assignment is applied immediately.
* A removed date-specific shift assignment falls back to the employee's **Default Work Schedule** for dates with no custom assignment.
* Custom download becomes available only after the **Check** step passes.
* Import results are shown after the CSV is processed.

#### Rules and behavior notes

* The system checks for conflicts before applying a shift change.
* A shift assignment can be blocked by a pending timesheet, a pending shift request, an overlapping approved or pending leave, or a closed pay run date.
* For multi-employee actions, valid items can proceed while blocked items are excluded.
* Dates in a closed pay run cannot be changed from the Shift module.
* When a custom download request is too large, the page requires a smaller range or narrower employee scope.
* The shift assignment import uses CSV only.
* The required import headers are **Employee Number / ID Number**, **Valid From**, **Valid Until**, and **Schedule Name**.
* **Schedule Name** in the import file can use a valid schedule name or **Mark as Rest Day**.

***

### Employee Calendar

The **Employee Calendar** page shows one employee's schedule across a four-week window. Use it when the weekly overview is too narrow and you need a broader schedule view for one employee before making a targeted change.

**Navigation:** Go to **Shifts → Shifts Overview**, then open the employee calendar from the employee's row.

#### What does the Employee Calendar display?

The calendar shows:

* Employee account details
* Four weeks of assigned shift entries by date
* Holiday overlays when applicable
* Leave overlays when applicable
* **Assign** and **Delete** actions for that employee

#### How do I use the Employee Calendar?

1. Open the employee's calendar from **Shifts Overview**.
2. Review the displayed date range and schedule pattern.
3. Check the employee's current assigned shifts alongside any holiday or leave context shown.
4. Use **Assign** or **Delete** if you need to make a direct employee-level update.

#### Rules and behavior notes

* Use **Employee Calendar** when the weekly overview is too narrow for the change you need to review.
* Assignment and deletion from this page still follow the same conflict checks used in **Shifts Overview**.

***

## Holiday Schedule

### Holiday Schedule

The **Holiday Schedule** page is used to maintain the company holiday calendar that affects how schedules, timekeeping, and payroll are interpreted on holiday dates.

Keep this page current before processing payroll or running attendance reviews for any period that includes holidays.

**Navigation:** Go to **Holiday Schedule**

#### What does the Holiday Schedule page display?

The page shows the company holiday list for the selected year, with controls to move between current, previous, and next year views where available.

Available actions on this page include adding, editing, and deleting individual holiday records, downloading the holiday list, and navigating to the import page.\
\
The page shows the holiday list for the selected year.

Each holiday record shows:

* holiday name
* holiday date
* holiday type
* applicable location
* pay rates for:
  * **Unworked**
  * **Worked**
  * **Working on a Rest Day**
  * **Working Overtime**
  * **Working Overtime on a Rest Day**
  * **Working w/ NSD**

The page also gives you actions to add, edit, delete, download, and import holidays.

If the selected year still needs setup, the page opens with a year-setup prompt before the holiday list is finalized. If the year is already set up, the holiday list opens directly.

#### When should I set up the holiday calendar?

Review and complete the holiday calendar at the start of every year. This is an annual task, not a one-time setup.

At the start of each year:

* Confirm the default holiday calendar matches your company's holiday rules, or
* Import a custom holiday list, or
* Add or update holidays directly on the page.

Complete the yearly holiday setup before running payroll or relying on holiday-based schedule interpretation for that year. If the selected year has not yet been prepared, the page guides you through a yearly setup step before individual holidays can be reviewed or edited.

***

### How do I add or update a holiday?

1. Go to **Holiday Schedule**.
2. Choose the year you want to review.
3. If the year has not been set up yet, complete the yearly setup step first.
4. Use the add or edit action for the holiday record.
5. Enter the holiday details.
6. Save the record.

#### Fields

* **Holiday Name (\*)** — the label shown in the holiday list and used in schedule interpretation.
* **Holiday Date (\*)** — the date of the holiday.
* **Holiday Type (\*)** — defines the holiday category. Accepted types are: **Regular Holiday**, **Special Non-Working Holiday**, and **Special Working Holiday**.
* **Location** — applies the holiday to all company locations, or to specific configured locations only. Use specific locations only when the holiday applies to a subset of employees.

`(*) Required fields must be completed before saving.`

#### Image Placeholder

\[Image: Holiday Schedule page showing the holiday list, year selector, and the add or edit holiday form]

***

### How do I download the holiday list?

1. Go to **Holiday Schedule**.
2. Click the download action.
3. Choose **CSV** or **XLS** as the file format.

#### Image Placeholder

\[Image: Holiday Schedule page showing the download action and file format options]

***

### How do I import holidays?

Use the holiday import page when you need to add multiple holiday entries at once instead of creating them one by one. Import only adds new records — it does not update or delete existing holidays.

**Navigation:** Go to **Holiday Schedule → Import Holidays**

#### Steps

1. Go to the holiday import page.
2. Click **Download Template** to get the current CSV template.
3. Prepare your CSV using the required column headers.
4. Upload the file.
5. Review any validation feedback shown by the page.
6. Complete the import.

#### What does the import require?

* Upload CSV files only.
* Use the current template — do not modify the column headers.
* Holiday dates must belong to the current year or a future year.
* Holiday types in the import file must match the accepted values: **Regular Holiday**, **Special Non-Working Holiday**, or **Special Working Holiday**.

#### Fields

* **Holiday Name (\*)** — the label shown in the holiday list.
* **Holiday Date (\*)** — the date of the holiday.
* **Holiday Type (\*)** — sets the holiday category.
* **Location** — applies the holiday to all locations or to selected configured locations.

`(*) Required fields must be completed before saving.`

#### What happens after saving or importing?

* A saved holiday appears in the selected year's holiday list.
* Imported holiday rows are added through the holiday import flow after the CSV passes validation.

#### Rules and behavior notes

* The page supports yearly review and setup.
* Holiday import uses CSV only.
* Use the current template when preparing the import file.
* Holiday dates in the import file must belong to the current year or a future year.
* Accepted holiday types are **Regular Holiday**, **Special Non-Working Holiday**, and **Special Working Holiday**.
