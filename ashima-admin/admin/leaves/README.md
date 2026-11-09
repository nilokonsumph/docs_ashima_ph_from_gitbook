# Leaves

The **Leave** module is where administrators review leave applications, manage employee leave balances, file leave on behalf of employees, monitor leave activity, and export leave records in the Admin Portal.

This module covers two main areas:

1. **Leave Monitoring & History** — review current approved leave, check leave history across statuses, and use the leave calendar for date-based visibility.
2. **Leave Balance Management** — assign leave types, update balances, file leave on behalf of employees, cancel approved leave, and reconcile balance movements through the transaction ledger.

***

### What pages are available in the Leave module?

The main pages in the Leave module are:

* **Overview** — daily monitoring of current approved leave activity.
* **Leave History** — review of submitted and approved leave across statuses and date ranges.
* **Leave Balance** — the main balance-management and leave-assignment page.
* **Leave Balance Details** — the employee-specific leave workspace for filing, updating, and managing one employee's leave records.
* **Leave Details** — the edit page for a specific assigned leave record, used for direct balance corrections.
* **Leave Calendar** — date-based leave visibility in a monthly calendar format.
* **Transaction Ledger** — balance-reconciliation view for one employee and one leave type.

These pages work together. Use Overview and Leave History for monitoring. Use Leave Balance and its detail pages for assignment, correction, and filing. Use Leave Calendar for date-based planning. Use Transaction Ledger when a balance needs deeper reconciliation.

***

### Before you begin: key leave concepts

Review these terms before working in the Leave module.

* **Leave Type** — the category of leave an employee can file, such as vacation leave or sick leave. Leave types are configured at the company level before they can be assigned to employees.
* **Earned Leave** — leave credits that have been earned by the employee. This serves as the beginning balance when a leave type is assigned.
* **Adjustment Leave** — a direct correction to an employee's leave balance, used when a manual override is needed outside of the normal earn-and-use flow.
* **Used Leave** — the portion of the balance already consumed by approved leave applications.
* **Available Balance** — the usable leave credits remaining after earned, adjustment, and used values are applied.
* **Delete Only** — removes the active leave assignment while preserving historical records. Also rejects pending applications tied to that assignment when required.
* **Delete and Purge** — the stronger cleanup action. Removes the assignment and broader related records as part of deeper data cleanup. Use only when full removal is truly needed.

***

## Leave Monitoring & History

### Overview

The **Overview** page is the main leave-monitoring page for current approved leave activity. Use it for a quick daily or current-period view of who is on leave without going into full employee leave history.

**Navigation:** Go to **Leave → Overview**

#### What does this page display?

The page shows current approved leave activity filtered by date. It is used to see:

* who is on leave today or within the selected date range
* leave type breakdown for the current period
* leave activity across employees

#### What can I do on this page?

* Search or narrow the current leave listing by employee or leave type
* Review leave activity for the selected dates
* Start the leave export flow
* Download attachments linked to leave requests when available

#### Image Placeholder

\[Image: Leave Overview page showing current approved leaves, leave type filter, and download controls]

***

### Leave History

The **Leave History** page shows leave applications across different statuses and date ranges. Use it when you need to check the outcome of a leave request, review prior leave activity for audit or payroll purposes, or prepare a leave history export.

**Navigation:** Go to **Leave → Leave History**

#### What does this page display?

The page shows historical leave applications and lets you review:

* employee leave requests
* approval status
* leave dates and filed dates
* leave type
* filtered history across employees or periods

#### How do I review leave history?

1. Go to **Leave → Leave History**.
2. Use the available filters — employee, status, date range, and leave type.
3. Click **Search** to apply the filters.
4. Review the matching leave rows.
5. Open the employee history detail view for a deeper review of one employee's leave activity.

#### Image Placeholder

\[Image: Leave History page showing filters, status columns, and download action]

***

### Leave Calendar

The **Leave Calendar** page displays approved leave applications in a monthly calendar format. Use it for date-based leave planning and visibility.

**Navigation:** Go to **Leave → Calendar**

#### What does this page display?

The calendar shows approved leave entries by date and supports:

* monthly leave planning
* day-based leave review
* leave-type filtering
* day or month export

#### What can I do on this page?

* Move between months using the navigation controls
* Jump to a selected month or year
* Filter the calendar by leave type
* Open a day view or day modal to see leave details for a specific date
* Download day or month results

Day-level downloads narrow the export to the selected day only. This page focuses on approved leave entries — pending or cancelled leave does not appear here.

#### Image Placeholder

\[Image: Leave Calendar page showing month navigation, leave type filter, and day drill-down]

***

## Leave Balance Management

### Leave Balance

The **Leave Balance** page is the main balance-management and leave-assignment page. Use it to check which leave types are assigned to employees, review remaining credits, and manage assignments.

**Navigation:** Go to **Leave → Leave Balance**

#### What does this page display?

The page lists assigned leave balances by employee and leave type. The table shows:

* **Employee Details**
* **Leave Type**
* **Leave Units**
* **Earned Leaves**
* **Available Balance**
* **Pending Approval**
* **Accrual Date**
* **Transaction**

The bottom action bar shows **Download** and **Delete**, with **Delete** disabled until rows are selected.

#### How do I review leave balances?

1. Go to **Leave → Leave Balance**.
2. Search for an employee if needed.
3. Use **Sort By** to change the listing order.
4. Review the employee leave rows and balance information.
5. Open the employee detail page when you need to update balances or file leave on behalf of that employee.

From this page you can also assign a new leave type to an employee, open the per-employee transaction ledger, start the balance-list download flow, and delete assigned leave records when cleanup is needed.

#### Image Placeholder

\[Image: Leave Balance page showing employee leave rows, Create action, balance columns, and detail links]

***

### How do I assign a leave type to an employee?

Use the Leave Balance page to create a new leave assignment for an employee. This action initialises the leave balance record and the related ledger activity for that leave type.

**Navigation:** Go to **Leave → Leave Balance**

#### Steps

1. Go to **Leave → Leave Balance**.
2. Click **Create**.
3. Select the employee.
4. Select the leave type.
5. Enter the beginning balance and effective details.
6. Review the assignment carefully.
7. Click **Save**.

#### Fields

* **Employee Name (\*)** — searches for and selects the employee receiving the leave assignment.
* **Leave Type (\*)** — selects the leave type to assign.
* **Earned Leaves (\*)** — sets the leave credits already earned as of the enrollment date. This becomes the beginning balance.
* **Adjustment Description** — records the reason for the starting balance or manual adjustment.
* **Used Leaves** — records leave already used before this assignment starts.
* **Available Leave Balance** — shows the usable balance after the entered values are applied. This is a calculated display, not an editable field.
* **Effective Start Date** — controls when the employee can begin using the assigned leave.
* **Year / Month** — defines whether the waiting period from date hired is counted in years or months.
* **Waiting-Period Value** — sets how long from date hired the employee must wait before using the leave. Entering `0` means the leave is available immediately.

`(*) Required fields must be completed before saving.`

The system checks for duplicate assignments for the same employee and leave type. Some fields depend on the leave type setup and the employee's date hired.

#### Image Placeholder

\[Image: Assigned Leave modal showing employee search, leave type, earned leaves, adjustment description, and effective start date]

***

### Leave Balance Details

The **Leave Balance Details** page is the employee-specific leave workspace. Use it to review one employee's full leave picture, file leave on their behalf, update balance records, or manage assigned leave.

**Navigation:** Go to **Leave → Leave Balance → Leave Balance Details**

#### What does this page display?

The page shows leave information for one employee and includes:

* assigned leave balances
* leave history for that employee
* leave application actions
* delete and purge actions
* download actions

#### What can I do on this page?

* Review the employee's assigned leave balances
* Create additional leave assignments for the employee
* Open the leave details editor for a specific leave type
* File leave on behalf of the employee
* Cancel approved leave when the record is eligible
* Download balance or history details
* Delete or purge assigned leave balances

#### Image Placeholder

\[Image: Leave Balance Details page showing assigned leave records, Apply Leave action, and download actions]

***

### How do I file leave on behalf of an employee?

File leave from the employee's Leave Balance Details page. The system enforces the same leave rules and schedule checks that apply to employee-initiated applications.

**Navigation:** Go to **Leave → Leave Balance → Employee Details**

#### Steps

1. Open the employee's Leave Balance Details page.
2. Start the **Apply Leave** action.
3. Select the leave type.
4. Enter the leave dates and required leave details.
5. Upload supporting documents if required.
6. Wait for the system to check the employee's work schedule and leave rules.
7. Review the leave request carefully.
8. Click **Submit Leave**.

#### Fields

* **Leave Type (\*)** — the leave category to be filed.
* **Date From (\*)** — the first day of leave.
* **Date To (\*)** — the last day of leave.
* **Leave Details** — supporting leave information required by the selected leave type.
* **Attachments** — supporting files when documents are required by the leave type.

`(*) Required fields must be completed before submitting.`

#### What happens before the leave is submitted?

The page runs a leave-check process before saving the application. This check reviews:

* the employee's work schedule
* leave restrictions for the selected leave type
* overlaps with existing leave or approved leave
* holiday or rest day conditions on the selected dates
* payroll lock or restriction status

Leave requests can be blocked if the selected dates conflict with schedule or leave restrictions. Supporting files can be uploaded before or during the leave application flow.

#### Image Placeholder

\[Image: Apply Leave form showing leave type, leave dates, leave details, supporting files, and Submit Leave button]

***

### Leave Details

The **Leave Details** page is the edit page for a specific assigned leave record. Use it when the employee's leave balance needs a direct correction — earned, adjustment, or used leave — against the assigned record.

**Navigation:** Go to **Leave → Leave Balance → Details**

#### What does this page display?

The page shows one assigned leave record and includes:

* assignment settings and effective date behavior
* earned leave update action
* adjustment leave update action
* used leave update action
* direct link to the transaction ledger

#### How do I update earned, adjustment, or used leave?

1. Open the employee's Leave Details page.
2. Choose the correct action:
   * **Add Earned Leaves** — adds earned credits to the balance.
   * **Add Adjustment** — applies a direct correction to the balance.
   * **Add Used Leaves** — updates the used portion of the balance.
3. Enter the required value.
4. Review the effect on the employee's leave balance.
5. Click **Save**.

These updates post ledger entries and update the employee's leave balance immediately. A valid assigned leave record must exist before any update can be saved.

#### Image Placeholder

\[Image: Leave Details page showing Add Earned Leaves, Add Adjustment, and Add Used Leaves actions with the transaction ledger link]

***

### How do I delete assigned leave?

The Leave module has two delete-type actions with different outcomes. Choose carefully before proceeding.

**Navigation:** Go to **Leave → Leave Balance Details**

#### Delete Only

**Delete Only** removes the active leave assignment from the current list while preserving historical records. It also rejects any pending leave applications tied to that assignment when required by the system flow.

Use **Delete Only** when you want to remove the current active assignment but still need the historical context to remain intact.

#### Delete and Purge

**Delete and Purge** is the stronger cleanup action. It removes the assignment and broader related records as part of deeper data cleanup.

Use **Delete and Purge** only when full removal is truly needed. This action affects more than the visible balance row.

These two actions are materially different. When in doubt, use **Delete Only**.

#### Image Placeholder

\[Image: Leave Balance delete actions showing Delete Only and Delete and Purge options]

***

### How do I cancel approved leave?

Approved leave can be cancelled from the employee leave area when the record is still eligible for cancellation.

**Navigation:** Go to **Leave → Leave Balance Details**

#### Steps

1. Open the employee's Leave Balance Details page.
2. Locate the approved leave entry you want to cancel.
3. Select the approved item.
4. Click the **Cancel Approved** action.
5. Confirm the action.

A visible approved leave row is not always cancellable. The system checks the leave status and related conditions before allowing cancellation. If the action is not available for a specific row, the record may no longer be eligible based on its current state.

#### Image Placeholder

\[Image: Cancel approved leave action on the employee Leave Balance Details page]

***

### Transaction Ledger

The **Transaction Ledger** page is the balance-reconciliation view for one employee and one leave type. Use it when the visible balance needs deeper review — to see exactly which transactions produced the current balance.

**Navigation:** Go to **Leave → Leave Balance → View Transaction Ledger**

#### What does this page display?

The page shows all leave-balance transactions behind one assigned leave record, including:

* earned transactions
* adjustment transactions
* used leave transactions
* delete or purge-related balance effects
* overall balance movement for the leave type

#### What can I do on this page?

* Review ledger rows for the selected leave type
* Change the leave-type context where available to review a different leave type for the same employee
* Download the ledger in spreadsheet format

#### Image Placeholder

\[Image: Leave Transaction Ledger page showing transaction rows, leave type context, and download action]

***

### What download options are available in the Leave module?

The Leave module supports export from several pages. Each download targets a different scope.

| Download                             | What it covers                                        |
| ------------------------------------ | ----------------------------------------------------- |
| Leave overview or history export     | Company-level leave activity across employees         |
| Leave balance list export            | All assigned leave balances                           |
| Employee leave balance detail export | One employee's leave balance records                  |
| Employee leave history detail export | One employee's leave history                          |
| Leave calendar export                | Approved leave for a selected day or month            |
| Transaction ledger export            | Balance movement for one employee and one leave type  |
| Attachment download                  | Supporting files attached to submitted leave requests |

Some downloads use a **Check** or precheck step before the export proceeds. Some support CSV or XLS output. Attachment download is separate from report exports and only applies when supporting files exist.

#### Image Placeholder

\[Image: Leave download options showing export actions from History, Balance, Calendar, and Ledger pages]

***
