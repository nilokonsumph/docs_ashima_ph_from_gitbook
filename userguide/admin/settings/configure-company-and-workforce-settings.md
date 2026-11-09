# configure company and Workforce settings

## find a Workforce setting

use the **Workforce** settings group to create and maintain the master records used in employee setup.

the currently identified Workforce settings pages include:

* **Location and Worksite**
* **Government Registration**
* **Cost Center**
* **Project**
* **Department**
* **Job Position**
* **Employment Type**
* **Rank**
* **Announcements**

these pages create reusable records and defaults that later appear in employee profiles, workflow scope, filters, downloads, and reports.

***

## use Location and Worksite

use this page to create and maintain the company locations and worksites that can later be assigned to employees.

**navigation:** go to **Settings → Workforce → Location and Worksite**

## review saved Location and Worksite records

the page displays a searchable listing of saved locations and worksites.

it includes:

* a search field with autosuggest
* the paginated location listing
* create, update, and delete actions

## manage Location and Worksite

you can:

* create a new location or worksite entry
* open a location detail page
* update an existing location or worksite
* delete one or more location entries

## how do i create a location or worksite?

1. open **Location and Worksite**.
2. start a new location entry.
3. complete the name, description, address and required **Flag Type** described below.
4. choose **Save**. correct any required-field or duplicate-name error, then verify the new row. choose **Cancel** to close the form without creating a location.

## complete the Location and Worksite details

* **Name (\*)** — the location or worksite name used later in employee records and related pickers.
* **Location Description** — a short description for the site.
* **Street** — street-level address information.
* **City** — city value for the location.
* **State** — state or province value for the location.
* **Zipcode** — postal code for the location.
* **Flag Type (\*)** — the required location-type marker used by the settings page.

`(*) Required fields must be completed before saving.`

## verify the saved Location and Worksite

the new location becomes available in later employee and company setup pages that use location-based assignment.

## apply the Location and Worksite rules

* **Name** is required.
* **Flag Type** is required.

## remove a location or worksite

1. select the locations you intend to remove and choose **Delete**.
2. review the confirmation before continuing.
3. if Ashima lists locations with assigned employees, review each location and its employee count. assignments for **Active** or **Inactive** employees can block deletion; **End of Employment** assignments do not. an existing assignment with no employee status can also block it.
4. move the relevant employee assignments to the correct location, or deselect the blocked locations, then try again.
5. check the refreshed list after deletion. the removed location no longer appears as active, while its employment and history references are retained.

{% hint style="warning" %}
if any selected location has blocking assignments, none of the selected locations is deleted. resolve the displayed blockers before retrying the selection.
{% endhint %}

use **Excel** or **CSV** to download the location list.

## use Government Registration

use this page to maintain the company's required government registration information.

**navigation:** go to **Settings → Workforce → Company Profile → Government Registration**

## review saved Government Registration records

the page displays the current government registration details saved for the company.

## manage Government Registration

you can review and update the saved government registration information used across payroll and company records.

## verify the saved Government Registration

the updated registration information becomes the company-level reference used by related payroll and compliance pages.

## apply the Government Registration rules

* this page maintains company registration data rather than employee-level data
* changes here can affect documents and payroll processes that rely on company registration details

## use Cost Center

use this page to create and maintain the cost centers used for employee and payroll reporting.

**navigation:** go to **Settings → Workforce → Company Profile → Cost Center**

## review saved Cost Center records

the page displays a searchable list of saved cost centers and a details page for each entry.

## manage Cost Center

you can:

* create a cost center
* open a cost center details page
* update an existing cost center
* delete one or more cost centers

## apply the Cost Center rules

* cost centers are later used in employee records and downloadable reports
* deleting a cost center should be done carefully if the value is already assigned to employees

## use Project

use this page to create and maintain project records used across employee and company assignment workflows.

**navigation:** go to **Settings → Workforce → Company Profile → Project**

## review saved Project records

the page displays a searchable project list with create, detail, update, and delete actions.

## manage Project

you can:

* create a project
* open project details
* update project information
* delete one or more projects

## apply the Project rules

* projects created here become reusable values in related workforce workflows
* remove a project only after checking whether it is still assigned elsewhere

## use Department

use this page to create and maintain departments used across workforce records, workflow routing, and reports.

**navigation:** go to **Settings → Workforce → Department → Department Positions**

## review saved Department records

the page displays:

* a searchable department list
* autosuggest search support
* department detail access
* create, update, and delete actions

## manage Department

you can:

* create a department
* open a department details page
* update an existing department
* delete one or more departments

## complete the Department details

* **Department Name (\*)** — the department name that appears in workforce records and downstream filters.
* **Description** — optional department description.

`(*) Required fields must be completed before saving.`

## verify the saved Department

the department becomes available for use in employee records, filters, workflow setup, and other settings pages that target department.

## apply the Department rules

* **Department Name** is required.
* deleting a department removes it from the active settings list, so review whether it is still used in employee records or workflow scope settings first

## use Job Position

use this page to create and maintain job positions used in employee employment details and reports.

**navigation:** go to **Settings → Workforce → Employment Settings → Job Position**

## review saved Job Position records

the page displays:

* a searchable list of job positions
* autosuggest support
* a position detail page
* create, update, and delete actions

## manage Job Position

you can:

* create a job position
* open position details
* update an existing position
* delete one or more positions

## complete the Job Position details

* **Position Name (\*)** — the position label used in employee records.
* **Description** — optional position description.

`(*) Required fields must be completed before saving.`

## apply the Job Position rules

* **Position Name** must be unique when creating a new position
* position values created here are reused across employment records and reports

## use Employment Type

use this page to create employment types and define the default entitlements and contribution coverage tied to each one.

**navigation:** go to **Settings → Workforce → Employment Settings → Employment Type**

## review saved Employment Type records

the page displays:

* a searchable list of employment types
* an employment type details page
* create, update, and delete actions

the details page stores the entitlement and contribution flags tied to that employment type.

## manage Employment Type

you can:

* create an employment type
* define its default entitlement set
* define whether the type is covered by **SSS**, **PhilHealth**, and **HDMF**
* update an existing employment type
* delete one or more employment types

## complete the Employment Type details

* **Name (\*)** — the employment type name used in workforce records.
* **Description** — optional description for the employment type.
* **Entitlement** — default payroll and timekeeping eligibility flags for the type.
* **Contribution** — default statutory contribution flags for the type.

`(*) Required fields must be completed before saving.`

## understand how employment type supplies defaults

this page defines important default rules that later affect payroll and timekeeping.

an employment type can set default eligibility for items such as:

* overtime
* holiday pay
* night differential
* rest day
* de minimis
* basic pay
* leaves
* 13th month pay
* service charge
* hazard pay
* regular and special holiday handling
* **SSS**
* **PhilHealth**
* **HDMF**

these flags are important because they shape what the employee is normally entitled to before more specific compensation or payroll setup is applied at employee level.

## apply the Employment Type rules

* **Name** must be unique.
* deleting an employment type should be handled carefully because it can affect downstream employee setup.
* this page sets defaults. Employee-level setup can still add more specific values later in Workforce and payroll configuration.

## use Rank

use this page to create and maintain rank values used in employee records and settings rules that target rank.

**navigation:** go to **Settings → Workforce → Employment Settings → Rank**

## review saved Rank records

the page displays a rank listing, detail view, and create, update, or delete actions.

## manage Rank

you can:

* create rank values
* update existing ranks
* delete one or more ranks

## apply the Rank rules

* ranks created here are later used in workforce records and payroll-setting applicability rules
* some payroll settings use rank as a targeting field, so removing a rank can affect those rules

## use Announcements

use this page to create and maintain company announcements shown elsewhere in the portal.

**navigation:** go to **Settings → Workforce → Announcements**

## review saved Announcements records

the page displays:

* a searchable announcements list
* autosuggest search
* create, update, activate, and delete actions

## manage Announcements

you can:

* create an announcement
* edit announcement title and body
* set one announcement as active
* delete announcements that are no longer needed

## complete the Announcements details

* **Title (\*)** — required announcement title.
* **Body (\*)** — required announcement body.

`(*) Required fields must be completed before saving.`

## verify the saved Announcements

the announcement is stored as part of the company announcement list.

if you set an announcement as active, the page also deactivates the other announcements after saving the selected one as active.

## apply the Announcements rules

* both **Title** and **Body** are required
* setting an announcement as active is not the same as just editing it
* only one active announcement should be expected after the active action runs
