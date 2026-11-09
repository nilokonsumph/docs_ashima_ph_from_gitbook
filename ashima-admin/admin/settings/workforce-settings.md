# Workforce settings

### What pages are available in Workforce Settings?

Use the **Workforce** settings group to create and maintain the master records used in employee setup.

The currently identified Workforce settings pages include:

* **Location and Worksite**
* **Government Registration**
* **Cost Center**
* **Project**
* **Department**
* **Job Position**
* **Employment Type**
* **Rank**
* **Announcements**

These pages create reusable records and defaults that later appear in employee profiles, workflow scope, filters, downloads, and reports.

***

### Location and Worksite

Use this page to create and maintain the company locations and worksites that can later be assigned to employees.

**Navigation:** Go to **Settings → Workforce → Location and Worksite**

#### What does this page display?

The page displays a searchable listing of saved locations and worksites.

It includes:

* a search field with autosuggest
* the paginated location listing
* create, update, and delete actions

#### What can I do from this page?

You can:

* create a new location or worksite entry
* open a location detail page
* update an existing location or worksite
* delete one or more location entries

#### How do I create a location or worksite?

1. Open **Location and Worksite**.
2. Start a new location entry.
3. Complete the required fields.
4. Save the new location.

#### Fields

* **Name (\*)** — the location or worksite name used later in employee records and related pickers.
* **Location Description** — a short description for the site.
* **Street** — street-level address information.
* **City** — city value for the location.
* **State** — state or province value for the location.
* **Zipcode** — postal code for the location.
* **Flag Type (\*)** — the required location-type marker used by the settings page.

`(*) Required fields must be completed before saving.`

#### What happens after I save?

The new location becomes available in later employee and company setup pages that use location-based assignment.

#### Rules, warnings, or behavior notes

* **Name** is required.
* **Flag Type** is required.
* deleting a location removes it from the active settings list, so check whether it is still being used in employee records before removing it

#### Image Placeholder

\[Image: Location and Worksite listing showing search, active location records, and create or edit actions]

***

### Government Registration

Use this page to maintain the company's required government registration information.

**Navigation:** Go to **Settings → Workforce → Company Profile → Government Registration**

#### What does this page display?

The page displays the current government registration details saved for the company.

#### What can I do from this page?

You can review and update the saved government registration information used across payroll and company records.

#### What happens after I save?

The updated registration information becomes the company-level reference used by related payroll and compliance pages.

#### Rules, warnings, or behavior notes

* this page maintains company registration data rather than employee-level data
* changes here can affect documents and payroll processes that rely on company registration details

#### Image Placeholder

\[Image: Government Registration page showing company registration fields and save action]

***

### Cost Center

Use this page to create and maintain the cost centers used for employee and payroll reporting.

**Navigation:** Go to **Settings → Workforce → Company Profile → Cost Center**

#### What does this page display?

The page displays a searchable list of saved cost centers and a details page for each entry.

#### What can I do from this page?

You can:

* create a cost center
* open a cost center details page
* update an existing cost center
* delete one or more cost centers

#### Rules, warnings, or behavior notes

* cost centers are later used in employee records and downloadable reports
* deleting a cost center should be done carefully if the value is already assigned to employees

#### Image Placeholder

\[Image: Cost Center listing page showing saved cost centers and details access]

***

### Project

Use this page to create and maintain project records used across employee and company assignment workflows.

**Navigation:** Go to **Settings → Workforce → Company Profile → Project**

#### What does this page display?

The page displays a searchable project list with create, detail, update, and delete actions.

#### What can I do from this page?

You can:

* create a project
* open project details
* update project information
* delete one or more projects

#### Rules, warnings, or behavior notes

* projects created here become reusable values in related workforce workflows
* remove a project only after checking whether it is still assigned elsewhere

#### Image Placeholder

\[Image: Project settings page showing project list and create action]

***

### Department

Use this page to create and maintain departments used across workforce records, workflow routing, and reports.

**Navigation:** Go to **Settings → Workforce → Department → Department Positions**

#### What does this page display?

The page displays:

* a searchable department list
* autosuggest search support
* department detail access
* create, update, and delete actions

#### What can I do from this page?

You can:

* create a department
* open a department details page
* update an existing department
* delete one or more departments

#### Fields

* **Department Name (\*)** — the department name that appears in workforce records and downstream filters.
* **Description** — optional department description.

`(*) Required fields must be completed before saving.`

#### What happens after I save?

The department becomes available for use in employee records, filters, workflow setup, and other settings pages that target department.

#### Rules, warnings, or behavior notes

* **Department Name** is required.
* deleting a department removes it from the active settings list, so review whether it is still used in employee records or workflow scope settings first

#### Image Placeholder

\[Image: Department page showing the department list, search, and details access]

***

### Job Position

Use this page to create and maintain job positions used in employee employment details and reports.

**Navigation:** Go to **Settings → Workforce → Employment Settings → Job Position**

#### What does this page display?

The page displays:

* a searchable list of job positions
* autosuggest support
* a position detail page
* create, update, and delete actions

#### What can I do from this page?

You can:

* create a job position
* open position details
* update an existing position
* delete one or more positions

#### Fields

* **Position Name (\*)** — the position label used in employee records.
* **Description** — optional position description.

`(*) Required fields must be completed before saving.`

#### Rules, warnings, or behavior notes

* **Position Name** must be unique when creating a new position
* position values created here are reused across employment records and reports

#### Image Placeholder

\[Image: Job Position page showing position list and position detail access]

***

### Employment Type

Use this page to create employment types and define the default entitlements and contribution coverage tied to each one.

**Navigation:** Go to **Settings → Workforce → Employment Settings → Employment Type**

#### What does this page display?

The page displays:

* a searchable list of employment types
* an employment type details page
* create, update, and delete actions

The details page stores the entitlement and contribution flags tied to that employment type.

#### What can I do from this page?

You can:

* create an employment type
* define its default entitlement set
* define whether the type is covered by **SSS**, **PhilHealth**, and **HDMF**
* update an existing employment type
* delete one or more employment types

#### Fields

* **Name (\*)** — the employment type name used in workforce records.
* **Description** — optional description for the employment type.
* **Entitlement** — default payroll and timekeeping eligibility flags for the type.
* **Contribution** — default statutory contribution flags for the type.

`(*) Required fields must be completed before saving.`

#### What should administrators know about employment type entitlements?

This page defines important default rules that later affect payroll and timekeeping.

The current source shows that an employment type can set default eligibility for items such as:

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

These flags are important because they shape what the employee is normally entitled to before more specific compensation or payroll setup is applied at employee level.

#### Rules, warnings, or behavior notes

* **Name** must be unique.
* deleting an employment type should be handled carefully because it can affect downstream employee setup.
* this page sets defaults. Employee-level setup can still add more specific values later in Workforce and payroll configuration.

#### Image Placeholder

\[Image: Employment Type listing with employment type details showing entitlement and contribution selections]

***

### Rank

Use this page to create and maintain rank values used in employee records and settings rules that target rank.

**Navigation:** Go to **Settings → Workforce → Employment Settings → Rank**

#### What does this page display?

The page displays a rank listing, detail view, and create, update, or delete actions.

#### What can I do from this page?

You can:

* create rank values
* update existing ranks
* delete one or more ranks

#### Rules, warnings, or behavior notes

* ranks created here are later used in workforce records and payroll-setting applicability rules
* some payroll settings use rank as a targeting field, so removing a rank can affect those rules

#### Image Placeholder

\[Image: Rank settings page showing rank list and detail access]

***

### Announcements

Use this page to create and maintain company announcements shown elsewhere in the portal.

**Navigation:** Go to **Settings → Workforce → Announcements**

#### What does this page display?

The page displays:

* a searchable announcements list
* autosuggest search
* create, update, activate, and delete actions

#### What can I do from this page?

You can:

* create an announcement
* edit announcement title and body
* set one announcement as active
* delete announcements that are no longer needed

#### Fields

* **Title (\*)** — required announcement title.
* **Body (\*)** — required announcement body.

`(*) Required fields must be completed before saving.`

#### What happens after I save?

The announcement is stored as part of the company announcement list.

If you set an announcement as active, the page also deactivates the other announcements after saving the selected one as active.

#### Rules, warnings, or behavior notes

* both **Title** and **Body** are required
* setting an announcement as active is not the same as just editing it
* only one active announcement should be expected after the active action runs

#### Image Placeholder

\[Image: Announcements page showing announcement list, active status, and edit actions]
