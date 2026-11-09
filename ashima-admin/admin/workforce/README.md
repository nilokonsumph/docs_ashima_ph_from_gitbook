# Workforce

## Workforce Module

The **Workforce** module is where administrators create and maintain employee records used across the entire Admin Portal. Every other module — payroll, timekeeping, leave, shifts, and workflow — reads from the employee record built here.

This module is used in this order:

1. **Find the employee** — use Employee Directory or Employee 201 to locate the record you need.
2. **Review or update personal and employment records** — use Personal Details and Employment Details for most direct record changes.
3. **Set up or update payroll configuration** — use Employee Compensation Details to set base pay, payroll group, entitlements, and statutory settings.
4. **Use supporting record pages when needed** — open Employee Status, Confidential Details, Educational Background, or Employment History for targeted updates.

***

### What pages are available in Workforce?

| Page                              | What it is for                                                                                       |
| --------------------------------- | ---------------------------------------------------------------------------------------------------- |
| **Employee Directory**            | Searchable employee listing — the starting point for finding any employee                            |
| **Employee 201**                  | Broad employee record review page with workforce, payroll, and history context in one place          |
| **Personal Details**              | Employee personal profile — personal info, emergency contacts, dependents, notes, and mobile numbers |
| **Employment Details**            | Employment profile — job, department, employment type, government IDs, history, and workflow setup   |
| **Employee Compensation Details** | Employee payroll setup — base pay, payroll group, entitlements, statutory settings, and bank details |
| **Employee Status**               | Employment status updates and stop-status maintenance                                                |
| **Confidential Details**          | Confidential employee information and payroll-group pairing                                          |
| **Educational Background**        | Employee education records                                                                           |
| **Employment History**            | Single employment-history record detail view                                                         |
| **Workflow Approvers**            | Employee-level workflow approver review                                                              |
| **Payroll Group**                 | Employee payroll-group page                                                                          |
| **Termination**                   | Employee termination page                                                                            |
| **201 Files**                     | Employee file page                                                                                   |

Use Employee Directory or Employee 201 to find employees. Use Personal Details and Employment Details for most record updates. Use Employee Compensation Details for payroll setup. Use the remaining pages for targeted, specific updates.

***

### Before you begin: key workforce concepts

* **Employee Directory** — the main searchable workforce listing used to find employees by name, ID, or initial letter.
* **Employee 201** — the broad employee record page that brings workforce, payroll, and history information together in one view. Use it for an overview before moving into a more specific page.
* **Personal Details** — the profile area for personal information, notes, emergency contacts, dependents, and mobile numbers.
* **Employment Details** — the profile area for job, department, employment type, rank, government IDs, and related employment settings.
* **Employee Visibility** — the access rule that controls whether the current admin can open a specific employee's details. Employees outside the allowed scope are not accessible.
* **Payroll Group** — the payroll grouping assigned to the employee. This determines which payroll run the employee belongs to.
* **Base Pay** — the employee's main pay amount used as the basis for payroll computation.
* **Entitlement** — a yes/no payroll rule that controls whether a pay item or statutory component applies to the employee, such as overtime, holiday pay, or night differential.
* **Compensation History** — the employee's recorded basic-pay history, including previous and current pay values with effective dates.

***

### What should administrators know about compensation in Workforce?

Set up the employee's core payroll configuration in Workforce before managing employee-specific pay entries in Pay Check, Leave, or Shifts.

The employee compensation record stores:

* payroll group and pay schedule
* pay rate and base pay
* payment method and payroll bank account
* minimum wage earner setting
* statutory contribution settings (SSS, PhilHealth, HDMF)
* withholding-tax-related settings
* entitlement flags — overtime, holiday pay, night differential, rest day, De Minimis, leaves, 13th month, and statutory contributions

These settings determine how the employee is treated in payroll before any employee-specific earnings, deductions, contributions, leave balances, shifts, or payslips are added in their own modules.

On the live employee compensation page, you can review all of the following in one place:

* **Compensation Summary**
* **Compensation Details**
* **Compensation History**
* **Entitlements**
* **Holiday Entitlement**
* **Withholding Tax**
* **Bank Information**
* **Logs History**

If the payroll group, base pay, entitlement flags, or statutory settings are incorrect here, the issue carries into payroll, contributions, leave handling, and payslip output. Review this page carefully before the employee's first payroll run.

***

## Finding Employees

### Employee Directory

Use **Employee Directory** to find an employee and open the next workforce page from a searchable listing.

**Navigation:** Go to **Workforce → Employee Directory**

#### What does this page display?

The page shows the searchable employee directory for the current company scope, including:

* employee directory rows or cards
* employee count for the current scope
* search results by name or ID
* initial-letter filtering results
* manager and position context where available

#### How do I search or filter this page?

You can narrow the directory by:

* employee name
* employee ID
* initial letter

If no employees match the current search or filter, treat the result as a no-records state — not a page error.

#### What can I do from this page?

* Search for an employee by name or ID
* Filter by initial letter
* Review the current employee count
* Open an employee profile from a directory item

The employee list is limited to employees visible to the current admin scope. Data privacy settings also affect what the current user can review from the directory.

#### Image Placeholder

\[Image: Employee Directory page showing search field, employee count, initial-letter filter, and employee listing]

***

### Employee 201

Use **Employee 201** when you need the broadest employee record view — workforce details, payroll setup, and history information in one place. Use it to get an overview before opening a more specific page.

**Navigation:** Go to **Workforce → Employee 201**

#### What does this page display?

The page shows the employee's consolidated record snapshot, including:

* the top Workforce employee listing
* shortcut icons for **Personal Details**, **Employment Details**, **Workflow Approvers**, **Payroll Group**, **Termination**, and **201 Files**
* employee profile and account details
* employment details — department, cost center, location, employment type, rank, and payroll group
* payroll-related details from the employee payroll information record
* workflow columns — **Enable Workflow Approvals** and **Assign Workflow Approvers**
* compensation, contribution, tax, and entitlement columns across the employee list

#### What should I review here first?

When you open Employee 201, start by checking:

* the employee's assigned payroll group
* the employee's basic pay
* the employee's workflow-approval settings
* the employee's statutory and entitlement columns
* whether lookup-based values — department, rank, location, employment type — are resolving correctly
* whether the employee's payroll-linked settings match what you expect to see in Pay Check

This page is a summary and review page. It does not replace the specific edit pages such as Personal Details, Employment Details, or Employee Status. If a lookup-based value looks wrong here — department, cost center, location, rank, or payroll group — check whether the underlying Settings record is correct first.

#### Image Placeholder

\[Image: Employee 201 page showing the employee table, Workforce shortcut icons, and payroll-linked employee columns]

***

## Employee Record Pages

### Personal Details

Use **Personal Details** to review or update the employee's personal profile information.

**Navigation:** Go to **Workforce → Personal Details**

#### What does this page display?

The page has a list view and an employee profile view. The profile view shows sections for:

* personal information
* employee notes
* emergency contact
* dependents
* mobile numbers

#### How do I update personal details?

1. Open **Personal Details**.
2. Search for the employee you need.
3. Open the employee profile.
4. Choose the section you want to update.
5. Save the updated section.

Each section saves independently — you can update one section without changing the others.

#### What can I do from this page?

* Browse the personal-details list and open one employee profile
* Update personal information, notes, emergency contact, and dependents
* Add or change mobile numbers, including the primary mobile number
* Trigger password actions — password change or password recovery
* Download the personal-details list in spreadsheet format

#### What happens after I save?

The system updates the selected section and returns a success or validation response. The export filename uses the company name plus a timestamp.

Before saving, confirm the employee is still within your visible scope — profile access fails if the employee ID is invalid or the employee is outside the allowed visibility.

#### Image Placeholder

\[Image: Personal Details page showing employee list, profile sections, and section-level update actions]

***

### Employment Details

Use **Employment Details** to review or update the employee's employment setup, government IDs, job history, and workflow-related settings.

**Navigation:** Go to **Workforce → Employment Details**

#### What does this page display?

The page has a list view and an employee profile view. The profile view shows:

* employment metadata — job, department, employment type, rank, location, cost center
* government ID information
* workflow-related options and approval sections
* reports-to and direct-reports context
* job change history and employment-type change history
* pending or upcoming employment-type and job-position changes when present

#### How do I update employment details?

1. Open **Employment Details**.
2. Search for the employee you want to review.
3. Open the employee profile.
4. Update the needed employment section.
5. Save the change.

#### What can I do from this page?

* Review and update employment details and government IDs
* Open workflow-related options and reassign workflow groups
* Add job change history or employment-type change history
* Delete history rows
* Download the employment list in spreadsheet format

#### What should I know before making changes?

Employment updates are not just profile changes. They can affect payroll-linked setup — reports-to relationships, workflow reassignment, and rank-based payroll behavior such as 13th-month entitlement.

Key validation rules:

* Job-change history requires an effective date, job change code, rank, department, and at least one reports-to selection. The current and new position cannot be the same.
* Employment-type history requires an effective date plus current and new employment type values.
* The employee payroll cloud ID is validated for uniqueness before an update is accepted.
* History deletion requires selected history IDs.

#### Image Placeholder

\[Image: Employment Details page showing employment profile sections, government IDs, history actions, and workflow options]

***

### Employee Compensation Details

Use **Employee Compensation Details** to review or update the employee's payroll setup, entitlement rules, and statutory settings. This is the most important page to complete correctly before the employee's first payroll run.

**Navigation:** Go to **Workforce → Employee Compensation**

#### What does this page display?

The page displays and collects the employee's full payroll configuration:

* payroll group, pay rate, and pay schedule
* base pay and basic pay adjustment value
* tax status and payment method
* bank and bank account details
* statutory settings — SSS, PhilHealth, HDMF
* minimum wage earner setting
* entitlement flags
* contribution lookup results for SSS and PhilHealth
* HDMF voluntary and HDMF modified values when used
* compensation history and logs

#### How do I review or update employee compensation?

1. Open the employee's **Compensation** page.
2. Select the employee's **Payroll Group**.
3. Set the **Pay Rate** and **Pay Schedule**.
4. Enter the **Base Pay**.
5. Complete the payment, statutory, and contribution settings.
6. Review and set the entitlement flags.
7. Save the compensation update.

#### Fields

* **Payroll Group (\*)** — assigns the employee to the payroll grouping used for payroll runs.
* **Pay Rate (\*)** — sets how the employee is paid. Options include By Day, By Hour, By Month, By Half Month, By Week, By Units Produced, and By Sales Amount.
* **Pay Schedule (\*)** — sets the employee's payroll schedule. Options include Daily, Weekly, Monthly, and Semi Monthly.
* **Base Pay (\*)** — the employee's main pay amount used as the basis for payroll computation.
* **Basic Pay Adjustment** — stores the employee's current base-pay value in the record used for compensation history.
* **Tax Status** — the employee's tax status used for payroll treatment.
* **Payment Method** — how the employee is paid.
* **Bank / Bank Account** — employee payroll bank and account details when used.
* **Fixed SSS / Fixed PhilHealth / Fixed HDMF** — fixed statutory values when the employee uses fixed contribution treatment.
* **Minimum Wage Earner** — marks whether the employee is treated as a minimum wage earner for payroll purposes.
* **Entitlements** — turns payroll items on or off for this employee. Includes overtime, holiday pay, night differential, rest day, De Minimis, leaves, 13th month, service charge, hazard pay, and statutory contributions.
* **Timesheet Required** — sets whether the employee is expected to use timesheets for payroll processing.

`(*) Required fields must be completed before saving.`

#### What happens after I save?

The system saves three linked records together: the employee payroll information record, the employee payroll account record, and the employee's basic-pay adjustment record. When used during onboarding, the system also clears the onboarding session keys after a successful save.

#### What should I know about statutory and entitlement settings?

* SSS and PhilHealth contribution lookups are based on the employee's base pay and the active company contribution tables.
* HDMF Voluntary and HDMF Modified values are saved separately when those options are used.
* If Night Differential is enabled, the employee payroll record uses the standard time-bound night differential rule.
* If tax entitlement or expanded withholding tax is turned off, clear the related withholding-tax fields rather than leaving them active.

#### Image Placeholder

\[Image: Employee Compensation page showing payroll group, pay rate, base pay, statutory settings, and entitlement flags]

***

## Supporting Record Pages

### Employee Status

Use **Employee Status** when the main task is updating the employee's employment status — not broader employment profile updates.

**Navigation:** Go to **Workforce → Employee Status**

#### What does this page display?

The page shows the employee's current employment status and status-related update actions. It also surfaces plan-limit and payroll-check context used during status review.

#### What can I do from this page?

* Review the current employment status
* Update employment status to **Active**, **Inactive**, or **End of Employment**
* Update stop-status information separately from employment status

#### What should I know before changing status?

The system checks plan limits before accepting a status change. If the employee is included in an open pay run, the system blocks changing the status to **Inactive** or **End of Employment** until the employee is removed from or excluded from that pay run.

Stop status is updated separately from employment status — they are two distinct actions on this page.

#### Image Placeholder

\[Image: Employee Status page showing current status and status update actions]

***

### Confidential Details

Use **Confidential Details** to review or update employee information that is treated as confidential, including payroll-group pairing.

**Navigation:** Go to **Workforce → Confidential Details**

#### What does this page display?

The page shows the employee's confidential record values, the employee's current payroll group, available payroll groups, and the confidential credentials state including who last updated the settings.

#### What can I do from this page?

* Review confidential employee information
* Update confidential status and payroll-group pairing when allowed

#### What should I know before making changes?

This page requires confidential-data visibility in addition to normal workforce access.

If the employee is already included in an open pay run, the system blocks changing the confidential status until the employee is removed from or excluded from that run. The selected payroll group must match the confidential-status rules, and can also be blocked if the payroll group has reached its configured limit.

#### Image Placeholder

\[Image: Confidential Details page showing confidential fields and update action]

***

### Educational Background

Use **Educational Background** to review or update the employee's education records.

**Navigation:** Go to **Workforce → Educational Background**

#### What does this page display?

The page shows the employee's educational records across the supported attainment levels:

* Elementary
* Secondary
* Vocational
* College
* Graduate Studies

#### What can I do from this page?

* Review, add, edit, and delete education records
* Review the full education record list before editing or deleting a row

Each education category is validated separately before updates are accepted. Edit access depends on the employee-edit privilege.

#### Image Placeholder

\[Image: Educational Background page showing education rows and add or edit actions]

***

### Employment History

Use **Employment History** to open and review one employment-history record in detail.

**Navigation:** Go to **Workforce → Employment History**

#### What does this page display?

The page shows one employment-history entry and its related metadata, including resolved lookup labels for position, rank, department, cost center, and location. It also shows any direct reports attached to that history record.

#### What can I do from this page?

* Review one employment-history detail record
* Check linked employment metadata for that history entry
* Review the direct-reports context attached to that history record

A valid history ID is required. If the referenced history ID is invalid, treat that as a missing-record state rather than a general workforce error.

#### Image Placeholder

\[Image: Employment History page showing one employee history detail record with resolved lookup labels]

***

### What should administrators know about Workforce downloads?

The Workforce module supports list-level downloads on the following pages:

* **Personal Details** — exports the personal-details list in spreadsheet format
* **Employment Details** — exports the employment list in spreadsheet format

Review the listing and apply any filters before downloading to make sure the export covers the correct employee scope. Use the page-specific export action for the correct record type.

#### Image Placeholder

\[Image: Workforce list page showing the download action on the listing view]
