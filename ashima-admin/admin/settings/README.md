# Settings

The **Settings** workspace is the company-definition layer for the entire Admin Portal. Use it to create the master records, payroll backbone rules, payroll entry types, timekeeping rules, and schedule templates that all other modules depend on.

Settings changes are company-wide changes. A change here — to a department, a payroll group, a loan type, or a tardiness rule — affects every module and every employee that depends on that setting. Review each change carefully before saving.

Use the **Settings** workspace to define the company rules, payroll defaults, schedule rules, and reusable setup records used across the admin portal. This workspace is not limited to one route file. It includes the pages exposed from the gear-menu settings navigation, even when some pages are still being migrated into newer Laravel route groups.

This module follows 5 main stages:

1. **Set up company structure** — create the master records used in employee profiles and workflow scope, such as departments, positions, locations, employment types, and ranks.
2. **Set up payroll backbone rules** — define payroll groups, pay schedules, payroll calendars, pay rates, statutory tables, and tax rules.
3. **Set up payroll entry types** — create the deduction, loan, insurance, and other payroll-side types that can later be assigned to employees.
4. **Set up timekeeping and schedule rules** — define work schedules and the calculation settings used by Hours, Shifts, and payroll.
5. **Maintain cross-module defaults** — keep announcement, workflow-related, leave-related, and other shared settings aligned with company policy.

### What pages are available in Settings?

The Settings workspace is accessed through the gear-menu entry point and organised by left-side navigation groups.

The confirmed settings groups are:

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

This guide covers the settings groups with the strongest current coverage: Workforce, Leaves, Hours, Pay Check, and Shifts. Workflow and the remaining groups need a dedicated validation pass before they can be fully documented.

***

### Before you begin: key settings concepts

* **Company-defined type** — a reusable record your company creates, such as a loan type, insurance type, department, or payroll group. Created once, used repeatedly across employee records and payroll setup.
* **Default rule** — a company-level rule the system follows unless a more specific employee-level setup overrides it. For example, Employment Type sets default entitlements; individual employees can have those overridden later.
* **Reference table** — a statutory or predefined table used in payroll calculation, such as PhilHealth Tables or HDMF Tables. These are review pages — they expose the table the system reads, not a place to configure individual employees.
* **Payroll backbone** — the combined setup of Pay Schedule, Payroll Calendar, Pay Rate, and Payroll Group that payroll depends on before a pay run can be created.
* **Entitlement** — a payroll or timekeeping eligibility flag attached to an employment type or employee setup, such as overtime, holiday pay, leaves, or statutory contribution coverage.

***

### How Settings affects the rest of the portal

Every other module reads from Settings. The downstream relationships are:



* **Workforce** uses structure settings such as department, rank, job position, employment type, cost center, project, and government registration.
* **Hours** uses time-entry and overtime rules, and it also depends on the shift and payroll settings that control how logs are interpreted.
* **Pay Check** uses payroll groups, pay schedule, payroll calendar, pay rate, deduction types, tax rules, statutory tables, and retroactive or payroll-side settings.
* **Shifts** uses work schedule settings, night differential settings, holiday pay settings, rest day settings, and schedule request settings.
* **Leaves** depends on leave-related settings and also on payroll and schedule defaults when leave affects payroll.
* **Workflow** depends on structure settings and approval-related configuration that controls how requests move through the system.

That is why Settings changes should be treated as company-wide changes, not one-off employee edits.

### What should administrators know about the Settings workspace?

Use **Settings** as the company-definition layer for the rest of the portal.

In practice:

* **Workforce** uses structure settings such as department, rank, job position, employment type, cost center, project, and government registration.
* **Hours** uses time-entry and overtime rules, and it also depends on the shift and payroll settings that control how logs are interpreted.
* **Pay Check** uses payroll groups, pay schedule, payroll calendar, pay rate, deduction types, tax rules, statutory tables, and retroactive or payroll-side settings.
* **Shifts** uses work schedule settings, night differential settings, holiday pay settings, rest day settings, and schedule request settings.
* **Leaves** depends on leave-related settings and also on payroll and schedule defaults when leave affects payroll.
* **Workflow** depends on structure settings and approval-related configuration that controls how requests move through the system.

That is why Settings changes should be treated as company-wide changes, not one-off employee edits.
