# Deduction settings

### Government Loans

Use this page to create and maintain the government-loan types your company can assign later to employees.

**Navigation:** Go to **Settings → Pay Check → Deductions → Government Loans**

#### What does this page display?

The page displays:

* a searchable list of saved government-loan types
* autosuggest search
* a detail page for each loan type
* create, update, and delete actions

It also loads employee-group targeting options such as **Rank**, **Department**, and **Employment Type**.

#### What can I do from this page?

You can:

* create a government-loan type
* limit where it is applicable
* update an existing government-loan type
* delete one or more government-loan types

#### Fields

* **Loan Type (\*)** — the government-loan type name.
* **Applicable For** — the employee group the type applies to.
* **Rank** — optional rank targeting.
* **Department** — optional department targeting.
* **Employment Type** — optional employment-type targeting.

`(*) Required fields must be completed before saving.`

#### Rules, warnings, or behavior notes

* **Loan Type** is required.
* this page creates the reusable loan type only; the actual employee assignment still happens later in employee payroll setup
* target selections help control where the type can be used

#### Image Placeholder

\[Image: Government Loans page showing loan-type list, search, and create flow]

***

### Third-Party Loans

Use this page to create and maintain third-party loan types that can later be assigned to employees.

**Navigation:** Go to **Settings → Pay Check → Deductions → Third-Party Loans**

#### What does this page display?

The page displays:

* a searchable list of third-party loan types
* autosuggest search
* a loan detail page
* create, update, and delete actions

#### What can I do from this page?

You can:

* create a third-party loan type
* update its name or description
* delete unused loan types

#### Fields

* **Loan Type (\*)** — the third-party loan type name.
* **Description** — optional description for the loan type.

`(*) Required fields must be completed before saving.`

#### Rules, warnings, or behavior notes

* this page creates the loan type only; employee-level loan assignment happens later in payroll setup
* delete a loan type only after checking whether it is already being used in employee records

#### Image Placeholder

\[Image: Third-Party Loans page showing loan-type listing and details access]

***

### Insurance

Use this page to create and maintain insurance deduction types that can later be assigned to employees.

**Navigation:** Go to **Settings → Pay Check → Deductions → Insurance**

#### What does this page display?

The page displays:

* a searchable insurance list
* an insurance detail page
* create, update, and delete actions

#### What can I do from this page?

You can:

* create an insurance type
* set deduction amount and recurrence behavior
* update an existing insurance setting
* delete one or more insurance settings

#### Fields

* **Insurance Name (\*)** — the provider or insurance name. This must be unique among active records.
* **Insurance Type (\*)** — the insurance category. If you choose `others`, an additional value is required.
* **Other Insurance Type** — required when the selected insurance type is `others`.
* **Plan Details** — optional plan information.
* **Deduction Amount (\*)** — required amount, validated as a numeric value with up to 2 decimal places.
* **Recurring Payment (\*)** — controls whether the deduction runs once or repeats.
* **Recurring Type** — when recurring is enabled, this controls whether the schedule is by interval or by occurrence.
* **Deduction Schedule** — required for interval-based recurring deductions.
* **Payroll Schedule** — required for recurring deduction timing.
* **Start Date (\*)** — required for recurring and one-time setups.
* **End Date** — required for interval-based recurring deductions.
* **Number of Occurrence** — required for occurrence-based recurring deductions.

`(*) Required fields must be completed before saving.`

#### What happens after I save?

The insurance type becomes available as a reusable payroll deduction setting that can later be assigned to employees.

#### Rules, warnings, or behavior notes

* **Insurance Name** must be unique among active records.
* the page changes required fields depending on whether the deduction is recurring
* interval-based and occurrence-based recurring setups use different required scheduling fields

#### Image Placeholder

\[Image: Insurance settings page showing insurance list and deduction scheduling fields]

***

### Other Deductions

Use this page to create and maintain other company-specific deduction types.

**Navigation:** Go to **Settings → Pay Check → Deductions → Other Deductions**

#### What does this page display?

The page displays:

* a searchable list of other deduction types
* autosuggest search
* create and delete actions
* employee-group targeting options such as **Rank**, **Department**, and **Employment Type**

#### What can I do from this page?

You can:

* create a company deduction type
* define its amount and recurrence pattern
* limit the type to selected employee groups
* delete deduction types that are no longer needed

#### Fields

* **Deduction Name (\*)** — the deduction type name. This must be unique among active company deduction records.
* **Deduction Amount (\*)** — required numeric amount with up to 2 decimal places.
* **Applicable For (\*)** — the scope or employee grouping the deduction applies to.
* **Recurring (\*)** — controls whether the deduction is one-time or recurring.
* **Recurring Type** — required when recurring is enabled.
* **Occurrence Start Date** — required for one-time or occurrence-based setup.
* **Interval Schedule** — required for interval-based recurring setup.
* **Payroll Schedule** — required for interval-based or occurrence-based recurring setup.
* **Interval Start Date** — required for interval-based setup.
* **Interval End Date** — required for interval-based setup.
* **Number of Occurrence** — required for occurrence-based setup.
* **Occurrence Schedule** — required for occurrence-based setup.
* **Rank** — optional rank targeting.
* **Department** — optional department targeting.
* **Employment Type** — optional employment-type targeting.
* **Description** — optional notes for the deduction type.

`(*) Required fields must be completed before saving.`

#### Rules, warnings, or behavior notes

* one-time and recurring setups use different required fields
* this page defines the deduction type only; it does not by itself deduct from an employee until that setting is later used in employee payroll configuration
* recurrence choices control whether the deduction behaves as a single pay-date item or a repeating schedule

#### Image Placeholder

\[Image: Other Deductions page showing deduction list and recurring setup fields]
