# choose which pages an administrator can access

## choose which pages an administrator can access

you can grant and customize access to the pages and actions an administrator needs. page access can be customized for any administrator, regardless of the label selected under **Roles**.

**navigation:** **Control Center → Teams / Privilege** → administrator detail; use **Settings** to identify the destination

### grant or remove access

1. open the intended administrator and choose **Edit**.
2. search for the page or action the administrator needs.
3. move the required labels to **Selected Roles**, or move labels back to **Available Roles** to remove access.
4. choose **Update**, complete the confirmation, and check the saved result.

some pages and actions use separate permission labels. select only the access the administrator needs.

this section controls pages and actions. to give the administrator access to another business under the account, update **List of Companies** under [manage administrators and access](manage-administrators-and-access.md#page-203b-pages-admin-control-center-understand-access-md).

### read the label prefixes

prefixes help you recognize labels; they do not establish what a permission does.

| prefix                 | family                                                                |
| ---------------------- | --------------------------------------------------------------------- |
| W / W(s)               | Workforce / Workforce Settings                                        |
| L / L(s)               | Leave / Leave Settings                                                |
| H / H(s)               | Hours / Hours Settings                                                |
| P / P(e) / P(d) / P(s) | Paycheck / Paycheck Earnings / Paycheck Deductions / Payroll Settings |
| S / S(s) / S(h)        | Shift / Schedule Settings / Holiday Schedule                          |
| W(f)                   | Workflow                                                              |
| I(s) / A(s)            | Integration / Announcement                                            |
| UM / T(s)              | Upload Manager / Track Settings                                       |
| R / UT                 | Reports / Utility Reports                                             |
| api(s)                 | API Generation                                                        |

search for the exact full label, including its displayed wording. prefixes and names alone are not a grant.

### forward lookup: standalone Settings

this table covers the standalone **Settings** page. other setup destinations may appear elsewhere in Admin. each group below starts from **Settings**.

#### Settings → Workforce

use this table to compare each destination with its menu, destination, and action permission labels.

| destination             | menu visibility label        | destination label            | action label and use                                                                                                                               |
| ----------------------- | ---------------------------- | ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| Location & Worksites    | `W(S) > company profile`     | `W(S) > company profile`     | add/update locations: `W(S) > company profile edit`; delete locations: `W(S) > company profile delete`; details/download: `W(S) > company profile` |
| Government Registration | `W(S) > company profile`     | `W(S) > company profile`     | update registration: `W(S) > company profile edit`                                                                                                 |
| Cost Center             | `W(S) > employment settings` | `W(S) > employment settings` | create/update: `W(S) > employment settings edit`; delete: `W(S) > employment settings delete`; details/download: `W(S) > employment settings`      |
| Project                 | `W(S) > employment settings` | `W(S) > employment settings` | create/update: `W(S) > employment settings edit`; delete: `W(S) > employment settings delete`; details/download: `W(S) > employment settings`      |
| Departments             | `W(S) > employment settings` | `W(S) > employment settings` | create/update: `W(S) > employment settings edit`; delete: `W(S) > employment settings delete`; details/download: `W(S) > employment settings`      |
| Job Positions           | `W(S) > employment settings` | `W(S) > employment settings` | create/update: `W(S) > employment settings edit`; delete: `W(S) > employment settings delete`; details/download: `W(S) > employment settings`      |
| Employment Type         | `W(S) > employment settings` | `W(S) > employment settings` | create/update: `W(S) > employment settings edit`; delete: `W(S) > employment settings delete`; details/download: `W(S) > employment settings`      |

#### Settings → Leaves

use this table to compare each destination with its menu, destination, and action permission labels.

| destination       | menu visibility label   | destination label       | action label and use                 |
| ----------------- | ----------------------- | ----------------------- | ------------------------------------ |
| Leave Monetized   | `L(S) > leave settings` | `L(S) > leave settings` | update: `L(S) > leave settings edit` |
| Maternity Benefit | `L(S) > leave settings` | `L(S) > leave settings` | update: `L(S) > leave settings edit` |

#### Settings → Hours

use this table to compare each destination with its menu, destination, and action permission labels.

| destination | menu visibility label        | destination label            | action label and use                                                                                                                                                                                           |
| ----------- | ---------------------------- | ---------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Time Entry  | `H(S) > time entry settings` | `H(S) > time entry settings` | kiosk create/update/rotate; time-entry options and IP changes: `H(S) > time entry settings edit`; kiosk/IP deletion: `H(S) > time entry settings delete`; kiosk list/IP download: `H(S) > time entry settings` |
| Tardiness   | `H(S) > time entry settings` | `H(S) > time entry settings` | review/change tardiness configuration: `H(S) > time entry settings edit`                                                                                                                                       |
| Overtime    | `H(S) > overtime settings`   | `H(S) > overtime settings`   | enable/update: `H(S) > overtime settings edit`                                                                                                                                                                 |

#### Settings → Paycheck

use this table to compare each destination with its menu, destination, and action permission labels.

| destination                                | menu visibility label                                 | destination label                     | action label and use                                                                                                                                                                   |
| ------------------------------------------ | ----------------------------------------------------- | ------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pay Rate → Pay Rate Calculation            | `P(S) > pay schedule settings`                        | `P(S) > pay rate settings`            | save/update calculation, working days and advanced settings: `P(S) > pay rate settings edit`; delete pay rates: `P(S) > pay rate settings delete`; details: `P(S) > pay rate settings` |
| Pay Rate → Pay Rates (by Date Type)        | `P(S) > pay schedule settings`                        | `P(S) > pay rate settings`            | update rates/restrictions: `P(S) > pay rate settings edit`; delete restrictions: `P(S) > pay rate settings delete`                                                                     |
| Pay Groups                                 | `P(S) > pay schedule settings`                        | `P(S) > pay run settings`             | create/update pay group: `P(S) > pay run settings edit`; delete pay group: `P(S) > pay run settings delete`; details/download: `P(S) > pay run settings`                               |
| Earnings → Allowance                       | `P(E) > earnings settings`                            | `P(E) > earnings settings`            | create/update: `P(E) > earnings settings edit`; delete: `P(E) > earnings settings delete`; details: `P(E) > earnings settings`                                                         |
| Earnings → De Minimis                      | `P(S) > other deductions settings`                    | `P(E) > earnings settings`            | create/update: `P(E) > earnings settings edit`; delete: `P(E) > earnings settings delete`; details/download: `P(E) > earnings settings`                                                |
| Earnings → 13th Month                      | use the 13th month permissions in the reference below | `P(E) > earnings settings`            | update: `P(E) > earnings settings edit`                                                                                                                                                |
| Earnings → Hazardous Pay                   | `P(E) > hazard pay settings`                          | `P(E) > hazard pay settings`          | create/enable/update: `P(E) > hazard pay settings edit`; delete: `P(E) > hazard pay settings delete`; details: `P(E) > hazard pay settings`                                            |
| Earnings → Other Earning                   | `P(E) > earnings settings`                            | `P(E) > earnings settings`            | create/update: `P(E) > earnings settings edit`; delete: `P(E) > earnings settings delete`; details: `P(E) > earnings settings`                                                         |
| Earnings → Retroactive Pay                 | `P(E) > earnings settings`                            | `P(E) > earnings settings`            | update: `P(E) > earnings settings edit`                                                                                                                                                |
| Deduction → Government Loans               | `P(S) > other deductions settings`                    | `P(S) > other deductions settings`    | create/update: `P(S) > other deductions settings edit`; delete: `P(S) > other deductions settings delete`; details/download: `P(S) > other deductions settings`                        |
| Deduction → Third Party Loans              | `P(S) > other deductions settings`                    | `P(S) > other deductions settings`    | create/update: `P(S) > other deductions settings edit`; delete: `P(S) > other deductions settings delete`; details: `P(S) > other deductions settings`                                 |
| Deduction → Insurance                      | `P(S) > insurance settings`                           | `P(S) > insurance settings`           | create/update: `P(S) > insurance settings edit`; delete: `P(S) > insurance settings delete`; details/download: `P(S) > insurance settings`                                             |
| Deduction → Other Deductions               | `P(S) > other deductions settings`                    | `P(S) > other deductions settings`    | create/update: `P(S) > other deductions settings edit`; delete: `P(S) > other deductions settings delete`; details: `P(S) > other deductions settings`                                 |
| Contributions → Contribution Schedule      | `P(S) > contribution settings`                        | `P(S) > contribution settings`        | update schedule: `P(S) > contribution settings edit`                                                                                                                                   |
| Contributions → Contribution Rules         | `P(S) > contribution settings`                        | `P(S) > contribution settings`        | update earnings/adjustment rules: `P(S) > contribution settings edit`                                                                                                                  |
| Taxes → Withholding Tax Deduction Schedule | `P(S) > taxes settings`                               | `P(S) > taxes settings`               | add/update: `P(S) > taxes settings edit`; delete: `P(S) > taxes settings delete`; details: `P(S) > taxes settings`                                                                     |
| Taxes → Withholding Tax Contribution Rules | `P(S) > taxes settings`                               | no separate edit permission is listed | if editing is unavailable, ask the account owner or Ashima support to review the required access.                                                                                      |
| Payment Options                            | `P > paycheck`                                        | `P(S) > Payment Options`              | save/update bank settings: `P(S) > Payment Options settings edit`; details: `P(S) > Payment Options`                                                                                   |
| Post Payroll Adjustment                    | `P(S) > pay schedule settings`                        | `P(S) > pay rate settings`            | update: `P(S) > pay rate settings edit`                                                                                                                                                |
| Payroll Variance                           | `P(S) > pay schedule settings`                        | `P(S) > pay schedule settings`        | update warnings/pay-run settings: `P(S) > pay schedule settings edit`                                                                                                                  |

#### Settings → Notification Manager

use this table to compare each destination with its menu, destination, and action permission labels.

| destination  | menu visibility label              | destination label                          | action label and use                                                                                                                                                                          |
| ------------ | ---------------------------------- | ------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Announcement | `I(S) > integration settings`      | `I(S) > integration settings`              | create/update/set active: `I(S) > integration settings edit`; delete: `I(S) > integration settings delete`                                                                                    |
| API Settings | `api(s) > api generation settings` | account/company eligibility; see API guide | see [API credentials](../business-account-and-capacity/review-plan-capacity-and-company-counts.md#page-203l-pages-admin-control-center-api-credentials-md); menu label alone is insufficient. |

### reverse lookup: navigation by task family

find a label you already have and see the navigation destinations it can expose. these rows are **visibility only**, not edit/delete or approval authority. other account/company and menu conditions remain. deeper items can be represented by a parent navigation link.

#### Workforce (W): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                     | navigation destinations                                                                                                                            | effect                      |
| ------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- |
| `W > workforce`                 | Personal Details; Employment Details; Workflow Approvers; PayGroup; Reports To; Government ID (import); New Employee ID (import); Document Manager | navigation visibility only. |
| `W > employee directory`        | Employee Directory                                                                                                                                 | navigation visibility only. |
| `W > org chart`                 | Org Chart                                                                                                                                          | navigation visibility only. |
| `W > employee termination`      | Termination                                                                                                                                        | navigation visibility only. |
| `W > employee 201`              | 201 Files; Workforce (import)                                                                                                                      | navigation visibility only. |
| `W > employee basic pay`        | Compensation; Retroactive Pay; Bank Info (import); Overtime Fixed Rates                                                                            | navigation visibility only. |
| `W > compensation details edit` | Compensation History                                                                                                                               | navigation visibility only. |

#### Leave (L): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label           | navigation destinations                                                                                                                                                                                                                                                                           | effect                      |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------- |
| `L > employee leaves` | Leave Overview; Leave Calendar; Leave Balance; Leave history — All; Leave history — Approved; Leave history — Pending; Leave history — Cancelled; Leave history — Rejected; CTO Balance; Maternity Benefits; Previous SSS Contribution; Leave Transfer; Leave (import); Unassigned Leave (import) | navigation visibility only. |

#### Hours (H): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label | navigation destinations                                                 | effect                      |
| ----------- | ----------------------------------------------------------------------- | --------------------------- |
| `H > hours` | Timesheets; Attendance; Punctuality; Overtimes; Restday; Hours (import) | navigation visibility only. |

#### Paycheck (P): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                   | navigation destinations                                                                                                                                      | effect                      |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------- |
| `P > pay run`                 | Payroll; Year-End; Paycheck Surfacing; Payroll Lock                                                                                                          | navigation visibility only. |
| `P > payroll opening balance` | Beginning Balance; Previous 2316; Beginning Balance Import (import); Previous 2316 (import); Payroll Exclusion; Payroll Withholding Tax Adjustment; WT Fixed | navigation visibility only. |
| `P > contributions`           | SSS Contribution; HDMF Contribution; PHIC Contribution; SSS Rules; PHIC Rules; HDMF I Rules; HDMF II Rules                                                   | navigation visibility only. |
| `P > paycheck`                | Payment Options; Payroll Journal Entries                                                                                                                     | navigation visibility only. |

#### Paycheck Earnings (P(E)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                  | navigation destinations                   | effect                      |
| ---------------------------- | ----------------------------------------- | --------------------------- |
| `P(E) > employee allowance`  | Allowances; Allowance (import)            | navigation visibility only. |
| `P(E) > employee deminimis`  | De Minimis; De Minimis Balance (import)   | navigation visibility only. |
| `P(E) > earnings settings`   | Allowance; Other Earning; Retroactive Pay | navigation visibility only. |
| `P(E) > hazard pay settings` | Hazardous Pay                             | navigation visibility only. |

#### Payroll Settings (P(S)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                        | navigation destinations                                                                           | effect                      |
| ---------------------------------- | ------------------------------------------------------------------------------------------------- | --------------------------- |
| `P(S) > thirteenth month`          | 13th Month; 13th Month Adjustments (import)                                                       | navigation visibility only. |
| `P(S) > taxes settings`            | Withholding Tax; Withholding Tax Deduction Schedule; Withholding Tax Contribution Rules           | navigation visibility only. |
| `P(S) > pay schedule settings`     | Pay Schedule; Pay Rate Calculation; Pay Rates (by Date Type); Pay Groups; Post Payroll Adjustment | navigation visibility only. |
| `p(s) > payslip template settings` | Payslip Template                                                                                  | navigation visibility only. |
| `P(S) > other deductions settings` | De Minimis; Government Loans; Third Party Loans; Other Deductions                                 | navigation visibility only. |
| `P(S) > insurance settings`        | Insurance                                                                                         | navigation visibility only. |
| `P(S) > contribution settings`     | Contribution Calculation; Contribution Schedule; Contribution Rules                               | navigation visibility only. |

#### Paycheck Deductions (P(D)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                              | navigation destinations                     | effect                      |
| ---------------------------------------- | ------------------------------------------- | --------------------------- |
| `P(D) > employee other earnings`         | Other Earnings; Other Earnings (import)     | navigation visibility only. |
| `P(D) > employee government loans`       | Government Loans; Govt Loans (import)       | navigation visibility only. |
| `P(D) > employee third party deductions` | 3rd Party Loans; Third Party Loan           | navigation visibility only. |
| `P(D) > employee other deductions`       | Other Deductions; Other Deductions (import) | navigation visibility only. |
| `P(D) > employee_insurance`              | Insurance; Insurance (import)               | navigation visibility only. |

#### Shift (S): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                   | navigation destinations | effect                      |
| ----------------------------- | ----------------------- | --------------------------- |
| `S > employee shift`          | Shifts Overview         | navigation visibility only. |
| `S > shift overview calendar` | Shifts Planning         | navigation visibility only. |

#### Holiday Schedule (S(H)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label               | navigation destinations | effect                      |
| ------------------------- | ----------------------- | --------------------------- |
| `S(H) - holiday schedule` | Holiday Schedule        | navigation visibility only. |

#### Other Utilities: navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label               | navigation destinations             | effect                      |
| ------------------------- | ----------------------------------- | --------------------------- |
| `UT > Disbursement`       | Disbursement; Disbursement (import) | navigation visibility only. |
| `UT > document`           | Documents                           | navigation visibility only. |
| `UT > Support`            | Support                             | navigation visibility only. |
| `UT > Hours Tools`        | Excess Logs; Possible Errors        | navigation visibility only. |
| `UT > Shifts Tools`       | Shift History                       | navigation visibility only. |
| `UT > Audit trail Report` | Audit Trail                         | navigation visibility only. |
| `UT > Log Summary Report` | Log Summary                         | navigation visibility only. |

#### Workflow (W(F)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                | navigation destinations                                                     | effect                      |
| -------------------------- | --------------------------------------------------------------------------- | --------------------------- |
| `W(F) > workflow settings` | Workflow Approval (import); Workflow Task Settings; Manager Access Settings | navigation visibility only. |

#### Utility Reports (UT): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                      | navigation destinations         | effect                      |
| -------------------------------- | ------------------------------- | --------------------------- |
| `UT > attendance report`         | Attendance; Paid Hours          | navigation visibility only. |
| `UT > Head Count Report`         | Head Count                      | navigation visibility only. |
| `UT > Employee List Report`      | Employee List                   | navigation visibility only. |
| `UT > Leave Conversion Report`   | Leave Conversion; Forfeiture    | navigation visibility only. |
| `UT > Payroll Register Report`   | Payroll Register; 90k; Wtt Tool | navigation visibility only. |
| `UT > report accounting entries` | Accounting Entries              | navigation visibility only. |
| `UT > Cost Structure Report`     | Cost Structure                  | navigation visibility only. |

#### SSS Reports: navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label            | navigation destinations | effect                      |
| ---------------------- | ----------------------- | --------------------------- |
| `UT > report sss r-3`  | R3                      | navigation visibility only. |
| `UT > report sss r-5`  | R5                      | navigation visibility only. |
| `UT > report sss ml1`  | ML1                     | navigation visibility only. |
| `UT > report sss r-1a` | R1A                     | navigation visibility only. |

#### PhilHealth Reports: navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                  | navigation destinations | effect                      |
| ---------------------------- | ----------------------- | --------------------------- |
| `UT > report philhealth rf1` | RF1                     | navigation visibility only. |
| `UT > report philhealth er2` | ER2                     | navigation visibility only. |

#### BIR Reports: navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                | navigation destinations | effect                      |
| -------------------------- | ----------------------- | --------------------------- |
| `UT > report bir 1601c`    | 1601C                   | navigation visibility only. |
| `UT > report bir 2316 new` | 2316                    | navigation visibility only. |

#### HDMF Reports: navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label              | navigation destinations | effect                      |
| ------------------------ | ----------------------- | --------------------------- |
| `UT > report mrrf`       | MRRF                    | navigation visibility only. |
| `UT > report hdmf stlrf` | STLRF                   | navigation visibility only. |

#### Workforce Settings (W(S)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                  | navigation destinations                                                 | effect                      |
| ---------------------------- | ----------------------------------------------------------------------- | --------------------------- |
| `W(S) > company profile`     | Profile; Location & Worksites; Government Registration                  | navigation visibility only. |
| `W(S) > employment settings` | Cost Center; Project; Departments; Job Positions; Employment Type; Rank | navigation visibility only. |

#### Leave Settings (L(S)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label             | navigation destinations                                               | effect                      |
| ----------------------- | --------------------------------------------------------------------- | --------------------------- |
| `L(S) > leave settings` | Leave Settings; Leave Monetized; Maternity Benefit; ACL Settings; CTO | navigation visibility only. |

#### Hours Settings (H(S)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                  | navigation destinations | effect                      |
| ---------------------------- | ----------------------- | --------------------------- |
| `H(S) > time entry settings` | Time Entry; Tardiness   | navigation visibility only. |
| `H(S) > overtime settings`   | Overtime                | navigation visibility only. |

#### Schedule Settings (S(S)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                     | navigation destinations                                                                         | effect                      |
| ------------------------------- | ----------------------------------------------------------------------------------------------- | --------------------------- |
| `S(S) > work schedule settings` | Night Differential Settings; Holiday Pay Settings; Rest Day Settings; Schedule Request Settings | navigation visibility only. |

#### Integration (I(S)): navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                   | navigation destinations | effect                      |
| ----------------------------- | ----------------------- | --------------------------- |
| `I(S) > integration settings` | Announcement            | navigation visibility only. |

#### API Generation: navigation

use this table to match each displayed permission label with the navigation destinations it can expose.

| exact label                        | navigation destinations | effect                      |
| ---------------------------------- | ----------------------- | --------------------------- |
| `api(s) > api generation settings` | API Settings            | navigation visibility only. |

### reverse lookup: actions, links, and request scope

some tasks use separate permissions for viewing, editing, and deleting. select only the permissions required for the administrator's work.

#### To Do Approvals: actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                                                   | permission labels                                                                                                                                                                                                    | what it allows                                                                                                                                                             |
| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| to do timesheets (including rest day/holiday variants) | `to do > approval timesheets`                                                                                                                                                                                        | allows the all to do request scope for timesheets, including rest day/holiday variants, when that filter is selected. it does not itself confer workflow approval.         |
| to do overview                                         | `to do > approval leaves`; `to do > approval shifts`; `to do > approval termination`; `to do > approval disbursement`; `to do > approval 13 month`; `to do > approval maternity benefit`; `todo > approval document` | the corresponding label contributes to the request scope for each to do overview status indicator. these are not numeric badge counts or unconditional approval authority. |
| to do overtime                                         | `to do > approval overtime`                                                                                                                                                                                          | allows the all to do request scope when that filter is selected. Workflow eligibility remains separate.                                                                    |
| to do payroll                                          | `to do > approval payroll`                                                                                                                                                                                           | allows the all to do request scope when selected. Workflow approval eligibility remains separate.                                                                          |
| to do year-end                                         | `to do > approval end of year`                                                                                                                                                                                       | allows the all to do request scope when selected. Workflow approval eligibility remains separate.                                                                          |

#### Workforce (W): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                       | permission labels                                                                                   | what it allows                                                                                                                                                         |
| -------------------------- | --------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| employee invitation import | `W > workforce edit`                                                                                | required together with `W > workforce` to open/import employee invitations; not every workforce action.                                                                |
| add employee               | `W > workforce edit`                                                                                | controls add employee and submission availability. capacity and form validation remain separate. the workforce delete label is not an add employee permission.         |
| compensation               | `W > compensation details edit`; `W > compensation details delete`                                  | the edit label controls editing; the delete label controls history deletion. employment state and selection still apply. navigation uses the separate basic-pay label. |
| BIR 2316                   | `W > employee termination edit`; `UT > report bir 2316 new edit`; `UT > report bir 2316 new delete` | these permissions control the BIR 2316 report. they do not grant general access to termination functions.                                                              |

#### Leave (L): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task          | permission labels                                                               | what it allows                                                                                                                                          |
| ------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| leave balance | `L > can apply leave`; `L > employee leaves edit`; `L > employee leaves delete` | the application, edit, and delete labels supply the corresponding leave balance permissions. valid leave, employee scope, and workflow remain separate. |

#### Paycheck (P): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                    | permission labels                    | what it allows                                                                                                   |
| ----------------------- | ------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| employee profile header | `P > employee payslip`               | makes the payslip sub-menu link available in the employee profile header; not unconditional download permission. |
| WT fixed import         | `P > payroll opening balance edit`   | required for the WT fixed import; other validation remains.                                                      |
| previous employer 2316  | `P > payroll opening balance delete` | controls deletion of previous-employer 2316. editing/uploading is separate.                                      |

#### Paycheck Earnings (P(E)): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                      | permission labels                | what it allows                                  |
| ------------------------- | -------------------------------- | ----------------------------------------------- |
| allowance import          | `P(E) > employee allowance edit` | required for the allowance import action.       |
| de minimis balance import | `P(E) > employee deminimis edit` | required to open the de minimis balance import. |

#### Paycheck Deductions (P(D)): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                      | permission labels                                                                              | what it allows                                                                                                                                              |
| ------------------------- | ---------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| other earnings import     | `P(D) > employee other earnings edit`                                                          | required for the other earnings import action.                                                                                                              |
| employee other earnings   | `P(D) > employee other earnings delete`                                                        | controls delete. employee status and selection restrictions remain.                                                                                         |
| insurance import          | `P(D) > employee insurance edit`                                                               | required for the insurance import action.                                                                                                                   |
| employee insurance        | `P(D) > employee insurance delete`                                                             | controls delete. assignment and update are separate actions.                                                                                                |
| government-loan import    | `P(D) > employee government_loans edit`                                                        | required for the government-loan import action.                                                                                                             |
| government loans          | `P(D) > employee government loans delete`                                                      | controls Admin delete availability; manager employee-scope permissions are separate.                                                                        |
| other deductions import   | `P(D) > employee other deductions edit`                                                        | required for the other deductions import action.                                                                                                            |
| employee other deductions | `P(D) > employee other deductions delete`                                                      | controls delete. status and selection limits remain.                                                                                                        |
| third-party loans         | `P(D) > employee third party deductions edit`; `P(D) > employee third party deductions delete` | the edit label controls assignment/edit and the delete label controls deletion in Admin. migration and selection limits remain; manager access is separate. |

#### Shift (S): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                     | permission labels                                      | what it allows                                                                                                                                          |
| ------------------------ | ------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| flexible shift Settings  | `S > shift planning edit`; `S > shift planning delete` | the edit label controls add/edit; the delete label controls delete. default-row and validation restrictions remain.                                     |
| shifts overview/calendar | `S > employee shift edit`; `S > employee shift delete` | the edit label controls change/import; the delete label controls deletion in Admin. deletion requires an existing schedule; manager access is separate. |

#### Leave Settings (L(S)): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                       | permission labels              | what it allows                                      |
| -------------------------- | ------------------------------ | --------------------------------------------------- |
| accumulated leave settings | `L(S) > leave settings delete` | required to delete accumulated-leave settings data. |

#### Payroll Settings (P(S)): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                         | permission labels                       | what it allows                                                                |
| ---------------------------- | --------------------------------------- | ----------------------------------------------------------------------------- |
| pay schedules                | `P(S) > pay schedule settings delete`   | controls delete. view and create controls are separate.                       |
| payslip settings             | `p(s) > payslip template settings edit` | controls edit/update of the payslip template.                                 |
| 13th month adjustment import | `P(S) > thirteenth month edit`          | required for the 13th month adjustment import.                                |
| 13th month runs              | `P(S) > thirteenth month delete`        | controls delete. run lifecycle and current state remain separate constraints. |

#### Holiday Schedule (S(H)): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task             | permission labels                                                | what it allows                                                                 |
| ---------------- | ---------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| holiday calendar | `S(H) - holiday schedule edit`; `S(H) - holiday schedule delete` | the edit label is required to save; the delete label is required for deletion. |

#### Workflow (W(F)): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task              | permission labels                                                | what it allows                                                                                                          |
| ----------------- | ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Workflow settings | `W(F) >workflow settings edit`; `W(F) >workflow settings delete` | the edit label controls create/edit; the delete label controls delete. neither makes the user a current-level approver. |

#### Utility Reports (UT): actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                                | permission labels                                                                                          | what it allows                                                                                                                     |
| ----------------------------------- | ---------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| paid hours reconciliation report    | `UT > attendance report edit`; `UT > attendance report delete`                                             | the edit label controls employee-scope access; the delete label controls deletion. no additional calculation authority is implied. |
| employee list report                | `UT > Employee List Report edit`; `UT > Employee List Report delete`                                       | the edit label controls create/preview; the delete label controls delete. row selection and report validation remain.              |
| headcount report                    | `UT > Head Count Report edit`; `UT > Head Count Report delete`                                             | the edit label controls create; the delete label controls delete.                                                                  |
| leave conversion/forfeiture reports | `UT > Leave Conversion Report edit`; `UT > Leave Conversion Report delete`                                 | the shared edit/delete labels control create/delete on both report screens.                                                        |
| payroll register                    | `UT > Payroll Register Report edit`; `UT > Payroll Register Report delete`                                 | the edit label is required to save; the delete label is required to delete.                                                        |
| accounting entries report           | `UT > report accounting entries edit`; `UT > report accounting entries delete`                             | the edit label is required to save; the delete label is required to delete.                                                        |
| cost structure report               | `UT > Cost Structure Report edit`; `UT > Cost Structure Report delete`                                     | the edit label is required to save; the delete label is required to delete.                                                        |
| payroll variance                    | `UT > Payroll Variance Report`; `UT > Payroll Variance Report edit`; `UT > Payroll Variance Report delete` | the base label is required to open; the edit label to save; the delete label to delete.                                            |

#### SSS Reports: actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task     | permission labels                                          | what it allows                                                  |
| -------- | ---------------------------------------------------------- | --------------------------------------------------------------- |
| SSS r-1A | `UT > report sss r-1a edit`; `UT > report sss r-1a delete` | the edit label is required to save; the delete label to delete. |
| SSS R-3  | `UT > report sss r-3 edit`; `UT > report sss r-3 delete`   | the edit label is required to save; the delete label to delete. |
| SSS R-5  | `UT > report sss r-5 edit`; `UT > report sss r-5 delete`   | the edit label is required to save; the delete label to delete. |
| SSS ML1  | `UT > report sss ml1 edit`; `UT > report sss ml1 delete`   | the edit label is required to save; the delete label to delete. |

#### PhilHealth Reports: actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task            | permission labels                                                      | what it allows                                                  |
| --------------- | ---------------------------------------------------------------------- | --------------------------------------------------------------- |
| PhilHealth RF-1 | `UT > report philhealth rf1 edit`; `UT > report philhealth rf1 delete` | the edit label is required to save; the delete label to delete. |
| PhilHealth ER2  | `UT > report philhealth er2 edit`; `UT > report philhealth er2 delete` | the edit label is required to save; the delete label to delete. |

#### BIR Reports: actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task      | permission labels                                            | what it allows                                                  |
| --------- | ------------------------------------------------------------ | --------------------------------------------------------------- |
| BIR 1601C | `UT > report bir 1601c edit`; `UT > report bir 1601c delete` | the edit label is required to save; the delete label to delete. |

#### HDMF Reports: actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task       | permission labels                                              | what it allows                                                  |
| ---------- | -------------------------------------------------------------- | --------------------------------------------------------------- |
| HDMF MRRF  | `UT > report mrrf edit`; `UT > report mrrf delete`             | the edit label is required to save; the delete label to delete. |
| HDMF STLRF | `UT > report hdmf stlrf edit`; `UT > report hdmf stlrf delete` | the edit label is required to save; the delete label to delete. |

#### Other Utilities: actions and scope

use this table to match each task with its permission labels and the access those labels provide.

| task                | permission labels                                                | what it allows                                                                               |
| ------------------- | ---------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| employee documents  | `UT > document edit`; `UT > document delete`                     | the edit label controls create new; the delete label controls delete.                        |
| summary logs report | `UT > Log Summary Report edit`; `UT > Log Summary Report delete` | the edit label controls create; the delete label controls delete. report validation remains. |

### related articles

* [Settings overview](../../settings/start-here-configure-ashima.md)

***
