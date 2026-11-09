# configure manager and Admin My Team access

## define who a manager can see and what they can do

**navigation:** go to **settings→workflow→manager access settings**, then on the manager access overview click the employee row you want to configure. use **manager privileges** to set up and manage what a specific employee can see and do in the my team workspace.

every manager in my team has two things configured here:

* **who they can see** — the employees visible to them, controlled by turning on a visibility scope
* **what they can do** — the actions they can perform on those employees, controlled by turning on module actions

both must be set up. turning on a scope without enabling any actions gives the manager visibility but no ability to act. enabling actions without an active scope has no effect at all.

***

## choose the manager's employee scope

think of the setup as two questions you answer for each employee:

**1. who should this manager see?**

use **manager privileges** to control which employees a person can see and manage in the my team workspace, and what they are allowed to do with those employees.

when setting up a manager's access, you have two ways to define who they can see. choose whichever fits how your organisation works — or use both at the same time:

**option 1 - direct reports** the manager can see and manage the employees who report directly to them, based on the reporting lines set in employment details. you can extend this down up to 3 levels — so the manager can also see employees who report to their direct reports, and one level further down from there.

use this option when access should follow your reporting structure. the manager only sees people in their chain of command.

**option 2 - department** the manager can see and manage all employees in one or more selected departments, regardless of whether those employees report to them directly.

use this option when access should cover a whole department — for example, an hr manager or a team lead who needs visibility across an entire team, not just their direct reports.

***

**2. what should this manager be able to do with those employees?**

once you have decided which option to use, you also choose what the manager can **do** with those employees - view only, or a combination of view, add, edit, and delete actions across timesheets, leaves, overtime, shifts, and workforce records.

both the scope (who they see) and the actions (what they can do) must be configured. turning on a scope without enabling any actions gives the manager visibility but nothing to act on. enabling actions without an active scope has no effect.

for each active scope, choose the actions across five resource groups:

| resource group | what actions cover                                              |
| -------------- | --------------------------------------------------------------- |
| **hours**      | timesheet logs - view, add, edit, delete                        |
| **leaves**     | leave records - view, approve, reject                           |
| **overtime**   | overtime records - view, approve, reject                        |
| **shifts**     | shift assignments - view, edit                                  |
| **workforce**  | employee directory, personal details, employment details - view |

the manager only sees the sections and buttons that match the actions you enable. if you enable view only, they see the data but cannot add, edit, or delete. if you enable add, edit, and delete, those buttons appear in their portal.

***

## before you set up: key terms

* **visibility scope** - the group of employees the manager is allowed to see in my team
* **direct reports** - employees who report directly to the selected person, based on the "reports to" relationship in their employment details record
* **department targets** - the specific departments you select when using the department scope
* **module action** - a specific thing the manager can do, such as view, add, edit, or delete, within one resource group
* **multi-level direct reports** - extends the direct reports scope to include employees below the immediate direct reports, down to a set level depth (maximum level 3)
* **module action** — a specific task the person can perform under an active scope, such as view, add, edit, or delete. module actions are grouped by resource: **hours**, **leaves**, **overtime**, **shifts**, and **workforce**.
* **department targets** — the specific departments selected for the department scope. visibility is limited to these departments only.

***

| page                                     | what it is for                                                                          |
| ---------------------------------------- | --------------------------------------------------------------------------------------- |
| **team access overview**                 | the starting point - see all employees with active manager privileges setup at a glance |
| **manager privileges** (employee record) | configure scope and actions for one specific employee                                   |
| **direct reports view**                  | verify exactly which employees a manager can see through the direct reports scope       |
| **department employees view**            | verify exactly which employees a manager can see through the department scope           |

***

## how do i set up manager privileges for an employee?

**Navigation:** Go to **Settings → Workflow → Manager Access Settings**, then open the employee on the Manager Access overview.

this opens the employee's manager privileges page. go to the **my team access** tab - this is where all scope and action configuration lives.

the page shows two cards side by side: **direct reports** on the left and **department** on the right. each card has its own toggle, its own settings, and its own set of resource group action controls.

You can also start from **Workforce**:

1. go to **Workforce**.
2. select the employee.
3. open the employee profile.
4. click **My Team Access** in the employee navigation.

this takes you to the team-access setup for that specific employee.

## setting up direct reports scope

use **direct reports** when the manager should see and act on employees who report directly to them.

## configure direct reports access

1. in the **direct reports** card, turn the scope toggle **on.** the card shows **enabled : 0/18** when first turned on - this means scope is active but no actions are enabled yet.
2. under **hours**, **leaves**, **overtime**, **shifts**, and **workforce**, turn on the specific actions the manager should be able to perform. use **enable all** to turn on every action in a group at once.
3. if the manager should also see employees below their direct reports, turn on **enable multi-level direct reports** and set the **level depth** dropdown. then click **save drill-down** — this setting has its own save step. (Drill down up to 3 levels)
4. save the page.

the enabled count on the card updates as you turn actions on. for example, **enabled : 9/18** means 9 of the 18 available actions are active.

## result of direct reports scope

once saved, the manager sees their direct reports in my team and can perform the specific actions you enabled. if you enabled only view actions, they can look but not change anything. if you enabled add, edit, or delete actions, those buttons appear in their portal.

the manager's scope appears in **team access overview** under **visibility scopes** as **direct reports**, and the enabled actions appear under **scope direct to**.

***

## extending direct reports with multi-level access

by default, direct reports scope shows only the employees who report directly to the manager (level 1). use multi-level direct reports when the manager should also see employees further down the reporting chain.

| level depth setting | who the manager can see                                       |
| ------------------- | ------------------------------------------------------------- |
| **1 (direct only)** | employees who report directly to the manager only             |
| **2**               | direct reports + employees who report to those direct reports |
| **3**               | two levels down plus one more level - the maximum             |

{% hint style="warning" %}
**important:** after changing the multi-level toggle or the level depth dropdown, click **save drill-down** before saving the rest of the page. this setting has a separate save step. if you skip it, the level depth change does not apply.
{% endhint %}

***

## setting up department scope

use **department** when the manager should see and act on employees from specific departments — not based on reporting lines.

## configure department access

1. in the **department** card, turn the scope toggle **on**.
2. click **manage departments**.
3. select the departments to include. the card shows a count such as **selected 2 / 11** as you select.
4. under the resource groups, turn on the actions the manager should be able to perform. use **enable all** to turn on every action in a group at once.
5. save the page.

## result of department scope

once saved, the manager sees all employees in the selected departments and can perform the specific actions you enabled. the selected departments appear in **team access overview** under **department targets**, and the enabled actions appear under **scope department**.

***

## using both scopes together

you can turn on both **direct reports** and **department** for the same manager. each scope has its own independent set of actions — the actions you enable under direct reports only apply to the manager's direct reports, and the actions you enable under department only apply to employees in the selected departments.

for example: a manager might have view-only access to their direct reports, but full add, edit, and delete access to a specific department. set each scope independently to achieve this

***

## enable all and clear

**enable all** - turns on every action in that resource group for that scope in one click. use it when the manager should have complete access to a group, rather than selecting individual actions.

**clear** - removes every active action in that resource group for that scope. when you click **clear**, a confirmation modal appears: "this will disable \[n] module(s) in \[group name] and revoke access." click **yes** to confirm or **cancel** to keep the current settings. use clear when you need to reset a group and reconfigure it from scratch.

***

## what to check before you save

* the scope toggle is **on** for every scope you want active. actions enabled under an inactive scope have no effect.
* at least one action is enabled under each active scope. a scope with no actions gives the manager visibility but nothing to do.
* if you changed the multi-level direct reports setting, you clicked **save drill-down** before saving the page.

***

## review all configured manager access

use **team access overview** as your starting point for reviewing and managing manager privileges across all employees. it shows every employee who has at least one active scope, what their scopes are, and which actions are enabled — without opening individual records.

**navigation:** go to **manager privileges → team access overview**

## review saved manager and Admin My Team access records

| column                 | what it shows                                                      |
| ---------------------- | ------------------------------------------------------------------ |
| **employee**           | the employee with active manager privileges setup                  |
| **visibility scopes**  | the active scopes — **direct reports**, **department**, or both    |
| **scope direct to**    | the actions enabled under the direct reports scope, shown as chips |
| **department targets** | the departments selected for the department scope                  |
| **scope department**   | the actions enabled under the department scope, shown as chips     |

use the **employee name or id** search to find a specific employee. click any employee row to open their manager privileges record and make changes. use **download** to export the full list.

an employee only appears here when they have at least one active scope. if all scopes are turned off, they are removed from this list.

***

## verify which employees the manager can see

after configuring a scope, use the verification views to confirm the correct employees are visible before considering the setup complete.

**for direct reports scope:** go to the employee's **manager privileges** page, scroll to the **direct reports** card, and click **view all employees**. this shows the exact employees the manager can see through that scope.

**for department scope:** go to the employee's **manager privileges** page, scroll to the **department** card, and click **view all employees**. this shows every active employee in the selected departments.

if the result looks wrong — for example, too few employees show in the direct reports view — check the "reports to" relationships in employment details for those employees. the direct reports scope only pulls employees where the reporting line is correctly set up.

***

## verify what the manager sees in the portal

when the manager logs into the **manager portal** (`ep.ashima.ph`), they see only the sections and actions you enabled. nothing more appears.

the manager portal left navigation reflects the enabled actions:

| portal section | appears when                     | what the manager can do                                                                                                                        |
| -------------- | -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| **todo**       | any approval action is enabled   | review and approve or reject pending requests — timesheets, rest day, holiday, mobile clockin, open shifts, overtime, leave, shifts, maternity |
| **workforce**  | view workforce action is enabled | view employee directory, personal details, and employment details for their visible employees                                                  |
| **leaves**     | leave action is enabled          | view leave records across all, approved, pending, cancelled, and rejected statuses, plus leave balance                                         |
| **hours**      | hours action is enabled          | view timesheet logs, attendance, punctuality, restday, and overtimes                                                                           |
| **shifts**     | shift action is enabled          | view shift assignments                                                                                                                         |

the action buttons the manager sees inside each section depend directly on what you enabled. for example:

* view only → the manager sees the data but has no add, edit, or delete buttons
* add + edit + delete timesheet → **add timesheet** and **edit timesheet** buttons both appear on the timesheet logs page
* no actions enabled for a section → that section does not appear in the manager's nav at all

{% hint style="info" %}
**note:** the manager portal is separate from the admin portal. managers cannot see or change their own manager privileges setup — only admins can configure this.
{% endhint %}

\*\*\*

## allow an administrator to manage My Team Access

**admin my team access** controls whether an admin account can control the **my team access** path in the admin portal.

use this setting when you want an admin to open and manage employee-level team-access setup. this setting does not by itself define which employees are visible or what actions are allowed. Those are configured separately in **manager privileges**.

## distinguish the two access controls

* **admin my team access** — turn **my team access** on or off for eligible admin users and review the audit trail.
* **manager privileges** — a separate employee-level team setup page used when a person also needs team visibility configuration.

## understand the access terms

* **My Team Access** — the access switch that allows an eligible admin account to use the My Team access path.
* **eligible admin** — an active admin account that appears in the page list and can be switched on or off.
* **manager privileges** — a separate employee-level setup that controls team visibility and module actions for an employee record.
* **visibility scope** — the employee group the person is allowed to see.

## decide when to turn on My Team Access

**navigation:** go to **control center → admin my team access**.

this setting controls whether an eligible admin account can use the **my team access** path in the admin portal.

when **my team access** is turned on for an eligible admin account, that admin can be allowed to open the team-access setup path from employee records and use the related admin-side team-access pages available to that account.

in practice, this is the switch that gives the admin account access to the **my team access** feature path. It does not replace the separate employee-level setup that decides:

* which employees are visible
* which scope is active
* which module actions are allowed

use this setting when the goal is to give an admin account the right to access and manage team-access setup.

## how do i search or filter this page?

use **search admin name...** to find a specific admin in the list.

use the **audit trail** filters when you want to review changes:

1. enter a name in **filter user...** if needed.
2. set the date range.
3. click **apply**.

click **clear** to remove the audit filters.

## turn access on, off, or review its history

you can:

* turn my team access **ON** for an eligible admin
* turn my team access **OFF** for an eligible admin
* review the history of access changes in **Audit Trail**

## apply the eligibility and audit rules

* this page only lists eligible admin users.
* not every admin account in the company appears here.
* designated admins are not included in this list.
* the page only works for active admin records under the current payroll account.
* if the admin is not eligible, the setting cannot be updated.
* if there are no matching audit records, the page shows **no audit trail found.**

## what should you do after turning my team access on?

after turning **my team access** on, review whether that admin also needs separate employee-level team visibility setup.

if yes, continue to **manager privileges** for the related employee record. that is where you define:

* which manager-level modules the person can use
* whether **direct reports** is enabled
* whether **department** is enabled
* which departments are included, when department visibility is used
* whether direct-report drill-down is allowed

without that second step, the admin may have **my team access** turned on but still have limited or no employee-level team visibility.

## how do admins reach the team-access setup after this is enabled?

after **my team access** is turned on for an eligible admin account, the admin can open the related team-access setup from employee records where that path is available in the current admin session.

one admin workflow is:

1. go to **workforce**.
2. select the employee.
3. open the employee profile.
4. click **my team access** in the employee navigation.

this opens the team-access setup page for that employee.

## understand the combined access result

this setting is the first part of the process that allows an eligible admin account to work through the my team access path.

when it is turned on, the admin account can use the My Team access path available to admin accounts.

if a separate employee-level team setup also exists, the person can then be given access to employee views such as:

* employee-level my team access pages
* direct report review
* department-based employee review
* employee-level modules assigned in **manager privileges**

the final result for employee-level team visibility depends on both:

* **my team access** being turned on
* the correct **manager privileges** and visibility scopes being configured

## understand what the access switch does not grant

this page does not:

* make someone a manager
* assign reporting lines
* assign departments
* automatically open all manager-level modules
* automatically let the user see all employees

use it as the access switch, not as the full permission setup.

## review the My Team Access audit trail

use **audit trail** when you need to review when **my team access** was changed and who made the change.

## interpret the audit entries

the audit table displays:

* **change date/time**
* **user**
* **my team access**

## how do i review audit history?

1. open **admin my team access**
2. go to **audit trail**.
3. enter **filter user...** if needed.
4. set the date range.
5. click **apply**.

click **clear** to reset the filters.

## verify the saved access change

use it to confirm:

* who changed the access setting
* when the change was made
* whether the setting was updated within the selected date range

## troubleshooting

## what should i do if...

## **the employee does not appear in team access overview after saving.**

at least one scope toggle must be on. check the **direct reports** and **department** toggles on the employee's **my team access** tab. an employee only appears in the overview when at least one scope is active. enabling actions alone without an active scope does not create an entry.

## **module actions are on but the manager cannot perform them in their portal.**

the scope toggle for that scope must also be on. check the scope toggle — if it is off, the actions have no effect regardless of what is enabled under the resource groups.

## **the direct reports scope is on but the manager cannot see their direct reports.**

the direct reports scope reads the "reports to" relationship from employment details. if an employee's reporting line is not set up correctly in their employment record, they do not appear in the scope. open the direct reports view for the manager and check whether the expected employees appear. if they do not, update the "reports to" field in those employees' employment details.

## **multi-level direct reports is on but deeper-level employees are not visible.**

you must click **save drill-down** after changing the level depth - it is a separate save from the main page. if you saved the page without clicking **save drill-down** first, the level depth change was not applied. return to the employee's record, set the level depth again, click **save drill-down**, then save the page.

## **the department scope is on but no employees appear in the department view.**

check that the selected departments have active employees assigned to them in employment details. a department that exists in settings but has no employees assigned returns no results in the department scope

## continue in the affected module

* [manage administrators, companies, and page access](../../control-center/)
* [manage approval work in Todo](../../todo-workflow/)

## related guide

* [use Manager portal](../../../manager/portal/) — shows managers how employee scope and assigned actions appear in their own portal.
