# start here: configure Ashima

the **Settings** workspace is the company-definition layer for the entire Admin Portal. Use it to create the master records, payroll backbone rules, payroll entry types, timekeeping rules, and schedule templates that all other modules depend on.

Settings changes are company-wide changes. A change here — to a department, a payroll group, a loan type, or a tardiness rule — affects every module and every employee that depends on that setting. Review each change carefully before saving.

use the **Settings** workspace to define the company rules, payroll defaults, schedule rules, and reusable setup records used across the admin portal. the workspace includes the destinations exposed from the gear-menu Settings navigation.

this module follows 5 main stages:

1. **Set up company structure** — create the master records used in employee profiles and workflow scope, such as departments, positions, locations, employment types, and ranks.
2. **Set up payroll backbone rules** — define payroll groups, pay schedules, payroll calendars, pay rates, statutory tables, and tax rules.
3. **Set up payroll entry types** — create the deduction, loan, insurance, and other payroll-side types that can later be assigned to employees.
4. **Set up timekeeping and schedule rules** — define work schedules and the calculation settings used by Hours, Shifts, and payroll.
5. **Maintain cross-module defaults** — keep announcement, workflow-related, leave-related, and other shared settings aligned with company policy.

## find the setting you need

the Settings workspace is accessed through the gear-menu entry point and organised by left-side navigation groups.

the confirmed settings groups are:

* **Workforce** — structure records used in employee profiles and workflow scope
* **Leaves** — leave-related company controls
* **Hours** — time-entry, tardiness, and overtime rules
* **Pay Check** — payroll backbone, payroll-entry types, and tax and statutory tables
* **Shifts** — work schedule templates and shift-related calculation rules
* **Workflow** — approval-rule behavior for the Workflow and To Do workspace
* **Notification Manager**
* **Upload Manager**
* **Reports**
* **Document Manager**
* **Data Privacy**
* **Utilities**

Start with the setting that controls the task you need to change. Use the sections below to connect the saved company rule with the employee record, request, pay run, or report it affects.

***

## understand how settings take effect

* **Company-defined type** — a reusable record your company creates, such as a loan type, insurance type, department, or payroll group. Created once, used repeatedly across employee records and payroll setup.
* **Default rule** — a company-level rule the system follows unless a more specific employee-level setup overrides it. For example, Employment Type sets default entitlements; individual employees can have those overridden later.
* **Reference table** — a statutory or predefined table used in payroll calculation, such as PhilHealth Tables or HDMF Tables. These are review pages — they expose the table the system reads, not a place to configure individual employees.
* **Payroll backbone** — the combined setup of Pay Schedule, Payroll Calendar, Pay Rate, and Payroll Group that payroll depends on before a pay run can be created.
* **Entitlement** — a payroll or timekeeping eligibility flag attached to an employment type or employee setup, such as overtime, holiday pay, leaves, or statutory contribution coverage.

***

## connect settings to daily work

every other module reads from Settings. The downstream relationships are:

* **Workforce** uses structure settings such as department, rank, job position, employment type, cost center, project, and government registration.
* **Hours** uses time-entry and overtime rules, and it also depends on the shift and payroll settings that control how logs are interpreted.
* **Pay Check** uses payroll groups, pay schedule, payroll calendar, pay rate, deduction types, tax rules, statutory tables, and retroactive or payroll-side settings.
* **Shifts** uses work schedule settings, night differential settings, holiday pay settings, rest day settings, and schedule request settings.
* **Leaves** depends on leave-related settings and also on payroll and schedule defaults when leave affects payroll.
* **Workflow** depends on structure settings and approval-related configuration that controls how requests move through the system.

That is why Settings changes should be treated as company-wide changes, not one-off employee edits.

## check scope and timing before you save

use **Settings** as the company-definition layer for the rest of the portal.

in practice:

* **Workforce** uses structure settings such as department, rank, job position, employment type, cost center, project, and government registration.
* **Hours** uses time-entry and overtime rules, and it also depends on the shift and payroll settings that control how logs are interpreted.
* **Pay Check** uses payroll groups, pay schedule, payroll calendar, pay rate, deduction types, tax rules, statutory tables, and retroactive or payroll-side settings.
* **Shifts** uses work schedule settings, night differential settings, holiday pay settings, rest day settings, and schedule request settings.
* **Leaves** depends on leave-related settings and also on payroll and schedule defaults when leave affects payroll.
* **Workflow** depends on structure settings and approval-related configuration that controls how requests move through the system.

That is why Settings changes should be treated as company-wide changes, not one-off employee edits.

## use Settings with the affected modules

Settings owns the complete configuration procedure. the affected module explains how the saved choice changes day-to-day work and links back to the applicable Settings article.

| Settings family                          | affected work                                                                                        | continue in the module guide                                                                                                     |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| company structure and employment choices | employee records, reporting groups, leave defaults, schedules, and payroll grouping                  | [Workforce](../workforce/)                                                                                                       |
| Leave, CTO, and maternity                | eligibility, balances, requests, approvals, calculations, and payroll inputs                         | [Leaves and CTO](../leaves-cto/)                                                                                                 |
| Hours and time entry                     | clock capture, timesheets, tardiness, overtime, undertime, breaks, and payroll inputs                | [Hours](../hours/)                                                                                                               |
| Shifts, holidays, and rest days          | schedule context, date classification, attendance, premium work, and payroll                         | [Shifts](../shifts/)                                                                                                             |
| Paycheck settings                        | payroll structure, earnings, deductions, contributions, tax, warnings, payslips, and payment outputs | [Paycheck](../paycheck/)                                                                                                         |
| Workflow                                 | approval levels, approvers, employee routing, and Todo work                                          | [To Do and Workflow](../todo-workflow/)                                                                                          |
| manager and administrator access         | employee visibility, allowed actions, company access, and page access                                | [Control Center](../control-center/)                                                                                             |
| **API Settings**                         | company API credentials and eligibility                                                              | [manage API credentials in Control Center](../control-center/account-security-and-support/generate-or-remove-api-credentials.md) |

When a result looks different from the setting you expected, start with the affected module to identify the employee or record, then follow its link to the setting that controls the result.
