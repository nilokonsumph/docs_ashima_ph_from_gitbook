# Hours

The **Hours** module is where administrators review, correct, analyse, and export employee timekeeping data in the Admin Portal.

Use this module to manage time entries from initial review through correction and reporting. It also provides attendance drill-down pages for monitoring specific conditions such as absences, tardiness, and rest day work.

This module covers two main areas:

1. **Timesheet Management** — review and correct time logs, manage recalculation, and export timesheet data.
2. **Attendance & Punctuality Reporting** — review attendance exceptions by condition using the absence, no-show, tardiness, undertime, and related pages.

***

### What pages are available in the Hours module?

**Navigation:** Go to **Hours**

The main pages under **Hours** are:

* **Timesheet Logs** — the primary review and correction page for employee time entries.
* **Timesheet Analysis** — generates and stores possible error reports for grouped issue review.
* **Timesheet Absences** — shows employees with no valid attendance for the selected date.
* **Clocked In** — shows employees with recorded clock-ins.
* **No Show** — shows employees with no recorded clock-in within the expected schedule window.
* **Undertime** — shows employees with undertime records.
* **Early Birds** — shows employees who clocked in earlier than expected.
* **Tardy** — shows employees with tardiness records.
* **Restday Logs** — shows employees with rest day work records.

The attendance and punctuality pages (Absences through Restday Logs) follow the same general pattern: filter by date and employee, review a table focused on one condition, and download as Excel or CSV. Use them when you need a narrower view than the full Timesheet Logs page.

***

### Before you begin: key timekeeping concepts

Review these terms before working in the Hours module. They affect how you interpret and correct timesheet records.

* **Work Schedule** — the assigned shift that determines when an employee is expected to clock in and out. Timesheet entries are always interpreted against the assigned Work Schedule, not the raw punch times alone.
* **Missing Punch** — one or more expected time logs were not recorded for a shift.
* **Excess Log** — more punches were recorded than the shift requires.
* **Recalculation** — the process of re-interpreting timesheet logs against the current shift settings to produce updated attendance and pay values. Adding, editing, or deleting a timesheet entry triggers recalculation for the affected dates.
* **PPA (Post Payroll Adjustment)** — the process for handling timesheet corrections after the connected payroll has already moved past the open review stage. Some timesheet changes are still permitted after payroll closes if they qualify under PPA rules.

***

## Timesheet Management

### Timesheet Logs

The **Timesheet Logs** page is the main review and correction page for employee time entries. Use it to review the timesheet listing, identify entries that need attention, and add, edit, or delete records as needed.

**Navigation:** Go to **Hours → Timesheet Logs**

#### What does the Timesheet Logs page display?

The page header shows **Timesheet Logs** and the active filter scope, which defaults to **Timesheet Entries on Last 6 Months** when no date filter is applied.

The main table displays:

* **Employee Details**
* **Date**
* **Clock In & Out**
* **Lunch Break Out & In**
* **First Break Out & In**
* **Second Break Out & In**
* **Hours Worked**
* **Tardiness (Min)**
* **Undertime & Absent (Min)**
* **Work Schedule**
* **Source**
* **Status**
* **Approved / Rejected By**
* **Reason**
* **Location**
* **Project**

If the current filters return no records, the page shows **no timesheet records for the selected filters.**

Use **Show Break Columns** to show or hide the break-related columns when the assigned shift does not use break punches.

#### What do the row status colours mean?

Each timesheet row is colour-coded to help you identify entries that need attention.

* **Orange** — the entry has missing logs, tardiness, undertime, or an absence. Review these rows first.
* **Red** — the schedule was changed after the employee clocked in.
* **Green** — the employee submitted an adjusted timesheet.
* **Blue** — an admin or HR initiated the entry through recalculation, update, or upload.
* **Purple** — the entry is a Post Payroll Adjustment (PPA).

The page also uses date accents for special day context:

* **Rest Day**
* **Regular Holiday**
* **Special Holiday**
* **Adjusted (MP)**

These indicators explain why a timesheet may be interpreted differently from a regular workday. Use the legend together with the row values to quickly identify entries that may need review.

#### What does the timesheet status panel show?

The status panel shows whether timesheet recalculation is currently needed.

* When the page is up to date, the panel shows **In Sync** with a **green light**. The **Recalculate** button is disabled.
* When queued recalculation is pending, the panel shows the pending count with a **red light**. The **Recalculate** button becomes available.

Check the status panel before reviewing or exporting timesheet data to make sure the records reflect the latest state.

#### How do I review the Timesheet Logs listing?

1. Go to **Hours → Timesheet Logs**.
2. Use **Search** to find a specific employee if needed.
3. Use **Sort By** to change the listing order.
4. Use **Show Break Columns** to show or hide break fields.
5. Check the status panel. If it shows pending recalculation, run **Recalculate** before continuing.
6. Review the row colours and values using the legend.
7. Select rows only if you plan to edit, delete, or export specific records.

#### How should I review a timesheet before making changes?

Before editing, deleting, or replacing a timesheet entry, review these items together:

* Compare the recorded log times against the assigned **Work Schedule**.
* Check whether the row shows missing punches, tardiness, undertime, absence, or other exceptions.
* Review **Hours Worked**, **Tardiness (Min)**, and **Undertime & Absent (Min)** before deciding whether a correction is needed.
* Review break fields when the assigned shift requires lunch or break punches.
* For overnight or cross-date entries, check both the date and time fields carefully.

If a timesheet looks incorrect even though the employee worked the full shift, check whether the assigned Work Schedule matches the timesheet date. A shift mismatch can produce undertime or other inaccurate results even when the employee rendered the correct hours. If the issue is caused by the shift assignment rather than the raw time logs, correct the shift first before changing the timesheet.

#### Image Placeholder

\[Image: Timesheet Logs page showing the search bar, sort control, Show Break Columns toggle, legend, status panel, and table columns]

***

### When should I use Recalculate on the Timesheet Logs page?

Use **Recalculate** when the status panel shows pending recalculation instead of **In Sync**. This processes queued timesheet updates before you continue with review or export.

Most timesheet updates trigger recalculation automatically. Manual recalculation is needed when the system has queued changes separately — for example, after a work schedule setting is updated after time logs were already captured, or after a larger recalculation run.

#### Steps

1. Go to **Hours → Timesheet Logs**.
2. Check the **Timesheet Status** panel.
3. If the panel shows pending recalculation, click **Recalculate**.
4. Wait for the process to finish. The page shows **Processing...** while recalculation runs.
5. Confirm the panel returns to **In Sync**.

#### What happens when I click Recalculate?

* The system begins the queued recalculation process.
* A progress modal appears showing **Please wait while we recalculate your data**.
* The footer shows **Recalculating timesheets...**
* When the run completes, the page shows **Successfully recalculated** and the status panel returns to **In Sync**.

#### Image Placeholder

\[Image: Timesheet status panel showing pending recalculation count, red light indicator, and the Recalculate button]

***

### How do I add a timesheet?

Use **Add Timesheet** when a manual time entry needs to be created for an employee. You can queue multiple entries for the same employee before saving.

**Navigation:** Go to **Hours → Timesheet Logs → Add Timesheet**

#### Steps

1. Go to **Hours → Timesheet Logs**.
2. Click **Add Timesheet**.
3. In **Choose Employee**, search for and select the employee.
4. Enter the **Shift Date** using the format MM/DD/YYYY.
5. Enter **Time In** and **Time Out**.
6. Complete the lunch or break fields only if the employee's schedule allows them.
7. Review the total hours shown for each row before saving.
8. Click **Add Row** if you need to queue another entry for the same employee.
9. Click **Save** when all entries are ready.

#### Fields

* **Choose Employee (\*)** — selects the employee whose timesheet logs will be added. Select the employee first — break field availability depends on the employee's assigned schedule.
* **Shift Date (\*)** — sets the work date for the timesheet entry. Use MM/DD/YYYY format.
* **Time In (\*)** — records the employee's start time.
* **Time Out (\*)** — records the employee's end time.
* **Lunch Out** — records the start of the lunch break. Only available when the assigned schedule allows it. Must be entered as a pair with Lunch In. Lunch times cannot match Time Out.
* **Lunch In** — records the end of the lunch break. Only available when the assigned schedule allows it.
* **1st Break Out** — records the start of the first break. Only available when the assigned schedule allows it.
* **1st Break In** — records the end of the first break. Only available when the assigned schedule allows it.
* **2nd Break Out** — records the start of the second break. Only available when the assigned schedule allows it.
* **2nd Break In** — records the end of the second break. Only available when the assigned schedule allows it.

`(*) Required fields must be completed before saving.`

#### What happens after I save?

* All valid queued entries are saved for the selected employee.
* Successfully saved rows are cleared from the queue.
* Rows with errors remain in the queue for correction.
* Adding a timesheet entry triggers recalculation for the affected employee dates.

#### What validation rules apply?

* Duplicate **Time In** and **Time Out** values for the same employee and date are blocked.
* **Shift Date** can only be moved within +/- 1 day of the original shift date when editing.
* Break fields are automatically cleared when the assigned schedule does not allow them.
* For night shift or cross-date entries, review both the date and time on each punch before saving.

#### Image Placeholder

\[Image: Add Timesheet page showing the employee selector, helper text, row entry table with time fields, Add Row button, and Save button]

***

### How do I edit or delete timesheet logs?

Use the selection controls on the **Timesheet Logs** page to correct or remove existing entries. Select one or more rows, then use the **Edit** or **Delete** action from the bottom action bar.

**Navigation:** Go to **Hours → Timesheet Logs**

#### Steps

1. Go to **Hours → Timesheet Logs**.
2. Select one or more rows using the checkbox column.
3. Check the **selected logs** count shown in the bottom action bar.
4. Click **Edit** to update the selected logs, or **Delete** to remove them.

**Edit** and **Delete** remain unavailable until at least one row is selected.

#### What should I know about editing?

The batch edit page lets you update multiple logs in one submission. After saving, recalculation runs automatically for the affected dates. The updated row becomes the active record used in review and payroll processing.

If a selected log cannot be edited, it is excluded from the editable set automatically. The page shows **Please select at least one log to edit** if no valid logs are selected.

Common reasons a log is unavailable for editing:

* Payroll is **Waiting for Approval** — add and edit actions are blocked.
* The date is closed and current PPA rules do not allow the change.
* The log already has a pending application.
* The log is already tagged for Post Payroll Adjustment (PPA).
* The employee or date is outside the allowed PPA period.

**Note on closed payroll:** A timesheet included in a closed payroll cannot be deleted. Use the eligible Post Payroll Adjustment (PPA) process when a correction is allowed.

#### What should I know about deleting?

The delete confirmation modal is titled **Delete Timesheet Logs**. It warns that deleting the selected logs **will trigger a recalculation for the affected dates.**

Use deletion only for eligible invalid, duplicate, or erroneous logs. A timesheet included in a closed payroll cannot be deleted; an eligible correction follows the Post Payroll Adjustment (PPA) process.

The page shows **Please select at least one log to delete** if no rows are selected.

#### Image Placeholder

\[Image: Delete Timesheet Logs modal showing the selected logs list and the recalculation warning]

***

### How do I download timesheet logs?

Use **Download** to export the current timesheet listing for audit, review, or offline analysis. Apply your filters before downloading so the export reflects the records you need.

**Navigation:** Go to **Hours → Timesheet Logs → Download**

#### Steps

1. Go to **Hours → Timesheet Logs**.
2. Apply the date range and filters you want included in the export.
3. Click **Download**.
4. Choose the file format: **Excel** or **CSV**.
5. Open **Advanced Options** if you want to set a timezone offset for the exported times.
6. Proceed to the custom field step if you want to add extra columns.
7. Complete the download.

#### What happens during the download?

The download modal is titled **Download Timesheets**. The flow prepares the export data first, then shows **Preparing download data...** before presenting the format and options steps.

If the result set is large, the page shows how many entries are included and splits the file automatically into parts, with each part covering a chunk range of up to 4,000 rows.

You can add up to three custom fields as extra columns in the downloaded file. The custom field prompt reads: **Want to include more details in your downloaded file? Choose up to 3 custom fields to add. These fields will be included as extra columns in your file.**

#### How do I adjust the timezone in the download?

Use the **Timezone** option in **Advanced Options** when you need the exported time values to reflect a different GMT offset — for example, when the receiving team reviews the file in a different timezone.

Select the preferred timezone offset (such as GMT+8 or GMT-5) before completing the download.

**Important:** The timezone setting adjusts the date and time values in the downloaded file only. It does not change the saved timesheet records in the portal, and it does not permanently update the employee's original time logs.

#### Image Placeholder

\[Image: Download Timesheets modal showing format selection, Advanced Options with timezone, and the custom field step]

***

## Attendance & Punctuality Reporting

### Timesheet Analysis

The **Timesheet Analysis** page generates and stores possible error reports for grouped timesheet issue review. Use it when you want to identify and track likely timesheet issues across a date range. Use **Timesheet Logs** when you need to correct the actual time entries.

**Navigation:** Go to **Hours → Timesheet Analysis**

#### What does this page display?

The page header shows **Possible Error Reports** and the description **Review generated timesheet issues and create new summaries.**

The report listing table shows:

* **Report Name**
* **Date From / To**
* **Include** — the issue types covered by the report
* **Created By**
* **Date Created**

Available actions are **Absent Report** and **Generate Report**.

#### How do I generate a timesheet analysis report?

Use **Generate Report** to create a saved report for possible timesheet issues across a selected date range.

1. Go to **Hours → Timesheet Analysis**.
2. Click **Generate Report**.
3. Enter the report name.
4. Select the date range.
5. Choose the issue types to include, such as tardiness, undertime, or missed punches.
6. Save the report.

A report requires a name, date range, and at least one included issue type. Some issue types use configured limits when the report is generated.

#### What can I do with a saved report?

* Open the saved report from the report listing to review the included issue categories and detail rows.
* Delete selected reports when they are no longer needed.
* Use **Absent Report** to move into attendance exception review.

#### Image Placeholder

\[Image: Timesheet Analysis page showing the generated report listing, Generate Report button, and Absent Report shortcut]

***

### Timesheet Absences

The **Timesheet Absences** page shows employees with no valid attendance for the selected date or date range. Use it to review who was absent, check for leave overlap, and download the absence listing.

**Navigation:** Go to **Hours → Timesheet Absences**

#### What does this page display?

The page shows the attendance section heading, a date-based heading such as **Absent Employees for \[Date]**, and the attendance table with pagination and download controls.

The attendance section tabs include:

* **Clocked In**
* **No Show**
* **Undertime**
* **Absent**

The table displays:

* **Employee Details**
* **Department | Position**
* **Work Schedule**
* **Phone Number**
* **Mobile Number**

#### How do I review absent employees?

1. Go to **Hours → Timesheet Absences**.
2. Use **Search Employee** to find a specific employee if needed.
3. Use the calendar control to set the date or date range.
4. Use **Schedule** and **Department** to narrow the listing.
5. Click **Show Leave** to load leave status information for the listed employees.
6. Review the table results.
7. Click **Download** to export the listing if needed.

#### Fields

* **Search Employee** — filters the listing by employee name.
* **Calendar** — sets the date or date range for the absence review.
* **Schedule** — filters the listing by work schedule.
* **Department** — filters the listing by department.
* **Show Leave** — loads leave status information to show whether an absence may already have filed leave tied to it.

Use **Show Leave** when you want to confirm whether an absence is a true absence or one that may already be covered by filed leave. This helps distinguish between employees who need follow-up and those who filed leave in advance.

#### Image Placeholder

\[Image: Timesheet Absences page showing the attendance tabs, search field, calendar, schedule and department filters, Show Leave button, and download action]

***

### Other Attendance and Punctuality Pages

The Hours module includes additional attendance listing pages that follow the same pattern as Timesheet Absences. Each page focuses on one condition, supports date and employee filters, and can be downloaded as Excel or CSV.

| Page             | What it shows                                                           |
| ---------------- | ----------------------------------------------------------------------- |
| **Clocked In**   | Employees with recorded clock-ins for the selected date                 |
| **No Show**      | Employees with no recorded clock-in within the expected schedule window |
| **Undertime**    | Employees with undertime records                                        |
| **Early Birds**  | Employees who clocked in earlier than their scheduled start             |
| **Tardy**        | Employees with tardiness records                                        |
| **Restday Logs** | Employees with recorded work on a rest day                              |

Use these pages when you need a narrower operational view than the full Timesheet Logs listing — for example, to follow up on a specific attendance condition or prepare a targeted export.
