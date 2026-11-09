# onboard employees

this guide covers everything administrators need to know when adding new employees to Ashima. Employee onboarding in Ashima is a structured, multi-step process that creates the employee record and prepares it for payroll, timekeeping, leave, and workflow use across the portal. Getting onboarding right from the start matters. Decisions made here - payroll group, pay calculation type, entitlements, contribution settings - flow directly into payroll runs, statutory deductions, and payslip output. A correctly set up employee record means fewer corrections later.

you can onboard employees one at a time through the guided employee creation flow, or upload many employees at once using **Bulk Employee Import**.

Two onboarding options are available: choose the onboarding path based on how many employees you need to add and how prepared your employee data is.

1. [**Individual employee onboarding**](onboard-employees.md#onboard-one-employee) — add one employee at a time through a three-step guided form.
2. [**Bulk Employee Import**](onboard-employees.md#bulk-employee-import) — upload multiple employee 201 records from a prepared CSV file.

## which onboarding option should i use?

| Path                                                                                         | Use when                                                               | How it works                                                                                                     |
| -------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| [**Individual onboarding**](onboard-employees.md#how-do-i-add-one-employee)                  | Adding one employee or a small number of employees.                    | Complete the employee record one screen at a time: Personal Details → Employment Details → Compensation Details. |
| [**Bulk Employee Import**](onboard-employees.md#how-do-i-onboard-multiple-employees-at-once) | Onboarding many employees or updating employee 201 records in batches. | Download the template, prepare employee rows, save as CSV, upload, and review validation results.                |

Individual onboarding is easier when you want to review each employee carefully as you go. Bulk onboarding is faster for larger groups, but requires stricter file preparation — the upload depends on exact headers, formats, and existing setup names.

## onboarding checklist

before you create a single employee record, take time to plan how new hires should be set up in Ashima. use this checklist before creating any employee record. Complete the setup items in Settings first - onboarding will fail or produce incomplete records if these are missing

## settings setup — complete before onboarding

* [ ] **Employment Types** created and entitlement defaults (i.e entitled to Overtime Pay) reviewed
* [ ] **Ranks** created and named consistently
* [ ] **Departments** created
* [ ] **Job Positions** created
* [ ] **Cost Centers** created (if used)
* [ ] **Projects** created (if used)
* [ ] **Locations / Worksites** created and named exactly as they will appear in employee records
* [ ] **Payroll Groups** created with the correct pay schedule and pay calculation type
* [ ] **Payroll Calendar** set up for each pay schedule
* [ ] **Pay Rate** configured
* [ ] **Statutory contribution settings** confirmed — SSS, PhilHealth, HDMF
* [ ] **Withholding Tax schedules** configured
* [ ] **Work Schedules** created and available for assignment after onboarding
* [ ] **Leave types** configured and ready to assign after onboarding
* [ ] **Workflow groups** created for the process types the employee will use
* [ ] **Employee Banks** added if bank account details will be entered during onboarding

## decisions to make before starting

* [ ] Which payroll group will the employee belong to?
* [ ] What is the employee's pay calculation type — monthly, daily, or hourly?
* [ ] Will the employee be included in the current payroll period or the next?
* [ ] What statutory contributions apply to this employee?
* [ ] What entitlements apply from day one — overtime, holiday pay, 13th month, leaves?
* [ ] Does the employee need a probationary period before certain entitlements begin?
* [ ] What work schedule will be assigned after onboarding?
* [ ] Does the employee need approvers set up for leave, overtime, or other request types?

## information to have ready

* [ ] Employee ID (confirm the company prefix and ID format)
* [ ] Full name, birth date, gender, marital status
* [ ] Contact details — email, primary mobile number
* [ ] Address
* [ ] Date hired, which may be scheduled for a future date, and employment type
* [ ] Department, job position, rank
* [ ] Reporting manager
* [ ] Government IDs — TIN, SSS, PhilHealth, Pag-IBIG, UMID
* [ ] Bank name and account number (if entering at onboarding)
* [ ] Monthly salary/Basic pay

## before you begin: confirm company setup

before onboarding any employee, confirm the company setup records they depend on already exist in Ashima. Missing setup values cause validation errors and leave the employee record incomplete after creation.

## confirm the following are already configured:

* Employment Type, Employment Status, Rank, Department, Job Position, Cost Center, Project, and Location Assigned
* Payroll Group, pay schedule, payroll calendar, and pay rate settings
* employee banks, if bank details will be entered during onboarding
* Statutory contribution settings for SSS, PhilHealth, and HDMF
* Shift, leave, earnings, deductions, and payroll entitlement settings
* Workflow setup, if the employee needs approvers for requests

for bulk onboarding, also read the upload rules in the Bulk Employee Import section before preparing your file.

## bulk employee import

## how do i onboard multiple employees at once?

use **Bulk Employee Import** to upload a CSV file containing multiple employee 201 records. The upload can create new employee records or update existing ones depending on whether the Employee ID already exists in Ashima.

**navigation:** Go to **Settings → Upload Manager → Workforce**

this process follows five steps:

1. open the **Bulk Employee Import** page under Upload Manager.
2. click **Download Template** and open the downloaded spreadsheet.
3. Prepare the employee rows — complete required fields, keep headers unchanged, and follow the required formats.
4. save the completed file as `.csv`.
5. Upload the CSV and review validation results before confirming.

## bulk upload rules

Follow these rules before preparing the file. Skipping them is the most common cause of blocked uploads.

* **Use the current template.** Select **Download Template** before preparing each upload. Keep the downloaded headers and required fields; an older saved copy may not match the current validation rules.
* **Do not change the headers.** Row 1 must stay exactly as downloaded. Do not rename, reorder, add, or delete columns.
* **Upload CSV only.** Prepare the file in the downloaded spreadsheet, then save as `.csv` before uploading.
* **Maximum 50 employees per file.** Split larger batches into separate files of 50 or fewer rows.
* **Maximum file size 10.0 MB.**
* **Avoid special characters.** Use plain letters or numbers for IDs and numeric fields unless the template field guide specifically allows another character.
* **Use exact existing setup names.** Fields such as Rank, Payroll Group, Location Assigned, and Employee Bank must match options already configured in Ashima unless the template notes that new entries can be added.

## how do i upload the file?

1. open **Bulk Employee Import**.
2. click **Browse File** and select the completed `.csv` file.
3. confirm the selected file name is displayed.
4. click **Upload File**.
5. review the validation result.

* if the file has both warnings and errors, the page displays separate lists for each.
* if the file contains warnings only (no errors), you can choose to continue processing the upload. Warnings do not stop the upload. You may review and correct them if needed, but you can also proceed without making changes.
* if the file contains errors, review the error list and update the source file. Save it again as a `.csv` and re-upload. You may still proceed, but any rows with errors will be skipped, and only valid rows will be processed.

{% hint style="info" %}
**important:** Review all validation warnings before continuing. Records with warnings will still be uploaded, while records with errors will be excluded from the upload.
{% endhint %}

## fields that must pass validation

these fields are required or have strict format rules. A missing, invalid, or mismatched value blocks the row from processing and being uploaded.

| Field                         | Required format or rule                                                                                                                                      |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Employee ID(\*)**           | Required for new employees. Must be unique in the file. Letters and numbers only. Allowed symbols: `*`, `_`, `-`, `/`, `\`. Avoid other symbols.             |
| **Email(\*)**                 | Required when used as the employee login identifier. Must be valid and unique.                                                                               |
| **Primary Mobile Number(\*)** | Required when used instead of email as the login identifier. Use numeric country-code format, such as `639171234567`. Numbers only avoids validation issues. |
| **Birthdate(\*)**             | Required. Use `MM/DD/YYYY` — for example, `02/25/1990`.                                                                                                      |
| **Employment Status(\*)**     | Required. Use **Active** or **Inactive**.                                                                                                                    |
| **Employment Type(\*)**       | Required for new employees. Must match an existing employment type.                                                                                          |
| **Date Hired(\*)**            | Required. Use `MM/DD/YYYY` — for example, `06/22/2015`.                                                                                                      |
| **Rank(\*)**                  | Required. Must match a default or existing rank in Ashima exactly.                                                                                           |
| **Payroll Group(\*)**         | Required for new employees. Must match an existing payroll group exactly.                                                                                    |
| **Entitled to Basic Pay(\*)** | Required. Use **Yes** or **No**.                                                                                                                             |

`(*) Required fields`

## recommended fields for clean onboarding

these fields may produce warnings rather than blocking errors, but completing them before upload reduces manual cleanup after onboarding.

| Field                                   | Format or rule                                                                                                                                                                                                            |
| --------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **First Name**, **Last Name**           | Maximum 50 characters each.                                                                                                                                                                                               |
| **Gender**                              | Use **Male** or **Female**.                                                                                                                                                                                               |
| **Marital Status**                      | Use: **Single**, **Married**, **Separated**, **Divorced**, or **Widow/er**.                                                                                                                                               |
| **Address**, **Province**, **City**     | Keep within the character limit shown in the template.                                                                                                                                                                    |
| **Tax Status**                          | Use a valid tax status from the template field guide.                                                                                                                                                                     |
| **Minimum Wage Earner**                 | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Basic Pay**                           | Required when Entitled to Basic Pay is Yes. Numbers only, up to two decimal places.                                                                                                                                       |
| **Bank Account**                        | Numbers only. No `+`, `-`, commas, or `#`.                                                                                                                                                                                |
| **Timesheet Required**                  | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to De Minimis**              | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Regular Holiday**         | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Unwork Regular Holiday.** | Use **Yes** or **No**. Yes, means the employee is paid his wage for that day even if he does not report to work. No, means the employee is not paid his wage for that day if he does not report to work (no work, no pay) |
| **Entitled to Special Holiday**         | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Unwork Special Holiday**  | Use **Yes** or **No**. Yes, means the employee is paid his wage for that day even if he does not report to work. No, means the employee is not paid his wage for that day if he does not report to work (no work, no pay) |
| **Entitled to Leaves**                  | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Night Differential**      | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Overtime**                | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to 13th Month**              | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Hazard Pay**              | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Service Charge**          | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to SSS**                     | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to PhilHealth**              | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to HDMF**                    | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Rest Day Pay**            | Use **Yes** or **No**.                                                                                                                                                                                                    |
| **Entitled to Tax**                     | Use **Yes** or **No** when the employee should be included in tax computation.                                                                                                                                            |

## optional fields and format notes

Add these when the data is already available. Including them during upload reduces manual setup after onboarding.

* **Middle Name** — optional.
* **Citizenship**, **Country** — optional. New entries may be added if they do not yet exist.
* **Dependents** — optional. Format: `First Name Last Name|MM/DD/YYYY|relationship`. Separate multiple dependents with a dash.
* **Job Position**, **Department**, **Cost Center** — optional. New entries may be added if they do not yet exist.
* **Location Assigned** — optional, but if entered it must match an existing location exactly.
* **Reports To (ID)** and **Reports To (Name)** — optional. Use an existing employee or an employee included in the same upload file.
* **UMID**, **TIN**, **SSS**, **PagIbig**, **PhilHealth** — optional. Numbers only. No `+`, `-`, commas, or `#`.
* **Employee Bank** — optional. If entered and not found in bank setup, the upload may show a warning.
* **SSS Settings** — optional. Accepted patterns: **table-based**, **table-based-ee**, or **fixed|amount**.
* **PhilHealth Settings** — optional. Accepted patterns: **table-based** or **fixed|amount**.
* **HDMF Settings** — optional. Accepted values: **Fixed**, **Base Pay**, or **Mixed Deduction**.
* **HDMF Percentage** — required when using a mixed HDMF setting. Numbers only.
* **Night Differential Rules** — use when Entitled to Night Differential is Yes. Accepted values: **Time Bound**, **Shift Restriction**, or **Fixed Lump Sum**.

## common upload errors and how to fix them

| Error                            | Fix                                                                                                                                         |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Incorrect template               | Download the latest template and do not change the header row.                                                                              |
| Too many rows                    | Split the upload into batches of 50 employees or fewer.                                                                                     |
| Wrong file type                  | Save as `.csv` before uploading.                                                                                                            |
| Invalid date                     | Use `MM/DD/YYYY`.                                                                                                                           |
| Duplicate Employee ID            | Make each Employee ID unique in the file and in Ashima.                                                                                     |
| Duplicate Email                  | Use a unique email address per employee.                                                                                                    |
| Invalid mobile number            | Use numbers only and remove all symbols.                                                                                                    |
| Rank does not exist              | Create the rank in Settings first, or use an existing rank name exactly as it appears.                                                      |
| Payroll Group does not exist     | Create or confirm the payroll group first, then use the exact name.                                                                         |
| Payroll Group cannot be changed  | For existing employees, the upload blocks payroll group changes when the employee has pending or open pay runs.                             |
| Location Assigned does not exist | Create the location in Settings first, or use an existing location name exactly.                                                            |
| Contribution setting not allowed | Check company contribution settings before uploading fixed or table-based contribution rules.                                               |
| Confidential access mismatch     | If your access is limited to confidential or non-confidential employees, the upload blocks updates to employees outside your allowed group. |

## onboard one employee

Steps 1 and 2 use **Next** to validate their current information and move forward; they do not create the employee. Complete step 3 and select **Onboard Employee** to create the record atomically. An invitation follows the commit and can fail separately from the saved record.

## how do i add one employee?

use individual onboarding when you are adding one employee or only a few and want to complete each record directly in the portal.

**navigation:** Go to **Workforce** and open the employee creation option.

the flow displays a three-step tracker: **Personal Details → Employment Details → Compensation Details**. Each step must pass validation before you can continue to the next. If you open step 2 or step 3 without completing the previous step, the system returns you to Personal Details.

after the Employee 201 choice screen, select **Required Fields Only** or **Full Onboarding**. This choice is part of individual onboarding and is not Bulk Employee Import; the current page does not define which fields are essential.

## step 1 — Personal Details

enter the employee's personal profile, contact information and address.

| Field                                                             | Notes                                                                   |
| ----------------------------------------------------------------- | ----------------------------------------------------------------------- |
| **Employee ID(\*)**                                               | Required. The form shows a company prefix beside the editable ID field. |
| **First Name**, **Last Name(\*)**                                 | Required.                                                               |
| **Middle Name**, **Suffix**, **Nickname**                         | Optional.                                                               |
| **Gender**, **Birth Date**, **Marital Status**                    | Personal profile fields.                                                |
| **Email**, **Primary Mobile Number**, **Secondary Mobile Number** | Contact information.                                                    |
| **Address**, **City**, **Province**, **Postal Code**, **Country** | Address fields.                                                         |

`(*) Required fields must be completed before saving.` click **Save and Continue** when personal details are ready. The system validates the information before moving to step 2. Correct any validation errors on the same page before continuing.

## step 2 — Employment Details

enter the employee's employment structure, reporting relationships, and government ID information.

| Field                                                                                           | Notes                                                                                                                |
| ----------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **Employee ID**                                                                                 | Carried forward from step 1. Read-only.                                                                              |
| **Location Assigned**, **Job Position**, **Project**, **Rank**, **Department**, **Cost Center** | Choose from the list of options you created on the settings.                                                         |
| **Employment Type (\*)**, **Date Hired (\*)**                                                   | Required.                                                                                                            |
| **Employment Status**                                                                           | The employee's current employment status.                                                                            |
| **Reports To**                                                                                  | Searchable reporting manager field. After selection, the page shows the manager's name, employee ID, and department. |
| **Government IDs**                                                                              | TIN, UMID, SSS No., Pag-IBIG No., and PhilHealth No.                                                                 |

if a required setup value is missing, the page provides setup links such as **+Add Location**, **+Add Job Position**, **+Add Rank**, and others. Use these to create the missing value without leaving the onboarding flow.

click **Save and Continue** after completing employment details. The system validates the employment information before moving to step 3.

`(*) Required fields must be completed before saving.`

## step 3 — Compensation Details

Complete the payroll setup for the employee. This step affects payroll computation, contributions, and pay-related reports — review it carefully before saving.

| Field                                           | Notes                                                                                                                                                                                                                    |
| ----------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Payroll Group (\*)**                          | Required. Drives the available Pay Schedule and Pay Calculation Type.                                                                                                                                                    |
| **Pay Schedule**, **Pay Calculation Type**      | Displayed from the selected Payroll Group.                                                                                                                                                                               |
| **Basic Pay**, **Daily Rate**, **Hourly Rate**  | Pay values used for payroll computation.                                                                                                                                                                                 |
| **Minimum Wage Earner**, **Timesheet Required** | Employee-level payroll settings.                                                                                                                                                                                         |
| **Entitlements**                                | Entitled to Basic Pay, De Minimis, Overtime Pay, Night Differential, 13th Month Pay, Hazard Pay, Service Charge, holiday pay, rest day pay, and leaves.                                                                  |
| **Contributions**                               | Entitled to SSS, PhilHealth, and HDMF. Includes SSS, PhilHealth, HDMF, HDMF voluntary, and HDMF modified settings. Contribution fields return lookup results depending on selected settings and the employee's base pay. |
| **Bank Information**                            | Employee Bank and Employee Bank Account No.                                                                                                                                                                              |

`(*) Required fields must be completed before saving.`

click **Save and Continue** to complete the employee creation. The system clears the stepper context after a successful save. Review the employee record in Workforce before the employee's first payroll run to confirm all personal, employment, compensation, contribution, and entitlement details are correct.

## onboarding & payroll setup for new hires: tips and best practices

before you create a single employee record, take time to plan how new hires should be set up in Ashima. The decisions below affect how employees are processed in payroll, what contributions are deducted, and what pay items they are entitled to. Making these decisions in advance - and creating the right setup in Settings before onboarding begins - saves significant time and avoids corrections mid-payroll.

## Decide whether new hires will be included in payroll immediately

Not every new hire should go into the next payroll run right away. Some employees join mid-period, some are on training, and some may need their payroll setup reviewed before their first run.

before onboarding, decide:

* **Will the employee be included in the current payroll period, or the next?** If they join after the pay period cutoff, it may be cleaner to include them in the following run.
* **Is the employee's payroll setup complete enough to run payroll?** The payroll group, pay calculation type, base pay, contribution deductions and entitlements all need to be correct before the employee is included in a pay run. If any of these are uncertain, complete the setup first.

## Consider whether new hires need their own payroll group

if your new hires are paid differently from your existing employees — for example, they are paid by hour or by day rather than by month, consider placing them in a separate payroll group rather than mixing them with your existing workforce.

A dedicated payroll group for new hires gives you:

* **A separate pay run.** You can process new hires independently without affecting your main payroll run until their setup is fully confirmed.
* **Different pay calculation rules.** Each payroll group carries its own pay calculation type. If new hires are paid hourly while existing employees are paid monthly, they need to be in different groups.
* **Cleaner payroll review.** Reviewing a smaller group of new hires separately is easier than filtering them out of a large masterlist.

Once a new hire's setup is confirmed and their payroll behavior is stable, you can move them into the main payroll group if that is appropriate for your company.

## Plan entitlement and contribution settings before creating the record

Entitlements and contribution settings are set at the employee level during onboarding. If different groups of employees are treated differently - for example, new hires are not yet entitled to rest day pay, or some employees are exempt from certain statutory contributions - plan these distinctions before you start creating records.

Consider the following before onboarding:

* **Statutory contributions (SSS, PhilHealth, HDMF).** Confirm which employees are covered and which are exempt. Set the contribution entitlements correctly during onboarding of new hires.
* **Overtime, holiday pay, night differential, and rest day pay.** If certain employees are not entitled to these from day one - for example, new hires under a specific employment type - set the entitlement flags to **No** at onboarding and update them when the entitlement period begins.

if a group of new hires has different entitlement rules from your existing employees, assign those settings individually for each employee rather than assuming the defaults will be correct. The Employment Type settings in Settings define company-level defaults - but individual employee compensation settings can override those defaults when needed.

## Set up individual employee settings before running payroll

after the employee record is created, and before the employee is included in their first payroll run, review and complete the following in the relevant modules:

* **Compensation Details** — confirm payroll group, pay calculation type, base pay, and all entitlement and contribution flags.
* **Shift assignment** — assign the correct work schedule in the Shifts module so timekeeping and attendance are interpreted correctly.
* **Leave balance** — assign the employee's leave types and opening balances in the Leave module if they are entitled from the start.
* **Workflow approvers** — confirm the employee is linked to the correct approval groups in Employment Details for the process types that apply to them.
* **Deductions and loans** — assign any recurring deductions or government loan deductions in Pay Check if they apply from the start.

## continue in the affected module

* [configure Workforce settings](../../settings/configure-company-and-workforce-settings.md)
* [assign shifts](../../shifts/)
* [assign leave or CTO](../../leaves-cto/)
