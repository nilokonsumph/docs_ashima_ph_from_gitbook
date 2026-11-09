# Hours settings

### What pages are available in Hours Settings?

Use the **Hours** settings group to control the company rules that affect how time entries, tardiness, and overtime are interpreted or processed.

The main pages in this settings group are:

* **Time Entry Option Settings**
* **Tardiness Settings**
* **Overtime Settings**

These settings connect directly to later attendance and payroll work:

1. Set the company time-entry capture and control rules.
2. Set the tardiness, undertime, and overbreak rules.
3. Set the overtime eligibility and threshold rules.
4. Let **Hours**, **To Do**, and **Pay Check** use those rules when logs are reviewed and payroll is calculated.

***

### What should administrators know about Hours setup?

Hours settings define the rule layer behind timekeeping.

These pages do not review attendance transactions one by one. Instead, they define how the system should interpret time entries later. In practice, they control:

* where employees are allowed to log time
* whether kiosk, IP, device, or pin-based controls apply
* whether tardiness logic is enabled
* how grace periods and rounding are applied
* when overtime becomes payable
* whether overtime needs approval or is capped

That is why changes here can affect attendance interpretation, payroll deductions, and payroll earnings at the same time.

***

### Time Entry Option Settings

Use **Time Entry Option Settings** to maintain the company controls for how employees are allowed to log time.

**Navigation:** Go to **Settings → Hours → Time Entry Option Settings**

#### What does this page display?

This page displays the company's time-entry control setup under **time entry option settings**.

The page includes company controls tied to:

* **Clock Guard** behavior
* company-approved **IP addresses**
* company **locations**
* **PIN code** lock behavior
* company **MAC address** or kiosk-related controls where used

#### What can I do from this page?

Use this page to:

* review the current clock-in restrictions
* maintain allowed IP addresses and location-linked time-entry points
* review kiosk-related setup where the company uses kiosk time entry
* review whether PIN-based lock behavior is enabled

#### Rules, warnings, or behavior notes

* changes here affect how time logs are accepted before admins ever review them in **Hours**
* location, device, IP, or kiosk restrictions can prevent a time entry from being treated as valid in the intended way
* this page is part of timekeeping control, not payroll calculation directly, but its settings still affect what attendance data payroll later receives

#### Image Placeholder

\[Image: Time Entry Option Settings page showing company time-entry rules and save controls]

***

### Tardiness Settings

Use **Tardiness Settings** to define how tardiness, undertime, and overbreak should be evaluated for the company.

**Navigation:** Go to **Settings → Hours → Tardiness Settings**

#### What does this page display?

This page displays the company's tardiness rule setup.

The rule groups include:

* the main **tardiness rule** on or off switch
* **daily grace period**
* **accumulated grace period**
* **tardiness rounding**
* **undertime rounding**
* **overbreak rounding**

#### What can I do from this page?

Use this page to:

* enable or disable company tardiness-rule handling
* define daily or accumulated grace-period behavior
* define rounding intervals for tardiness
* define rounding intervals for undertime
* define rounding intervals for overbreak

#### Rules, warnings, or behavior notes

* when the main tardiness rule is turned off, the company tardiness option rows are also disabled
* the page validates rounding ranges so the **from** value cannot be greater than or equal to the **to** value
* if daily grace is enabled, the grace minutes and grace start window become required
* if accumulated grace is enabled, the accumulated grace minutes become required
* changing these rules can trigger recalculation work for recent timesheet records because the company timing logic has changed
* these rules affect not only **Tardiness**, but also **Undertime** and **Overbreak** handling in attendance and payroll

#### Image Placeholder

\[Image: Tardiness Settings page showing the company tardiness rules used for hours and payroll]

***

### Overtime Settings

Use **Overtime Settings** to define when overtime starts, how much overtime can be counted, and whether special overtime controls apply.

**Navigation:** Go to **Settings → Hours → Overtime Settings**

#### What does this page display?

This page displays the company's overtime rule setup.

The fields in code show this page controls:

* whether overtime settings are enabled
* **overtime grace minutes**
* **minimum overtime minutes**
* whether an **overtime cap** is enabled
* the **overtime cap minutes**
* whether **pre-shift overtime** is enabled

#### What can I do from this page?

Use this page to:

* turn overtime-rule handling on or off
* define how many minutes must be reached before overtime is counted
* define the grace minutes around overtime
* cap overtime when company policy requires a maximum
* allow or disallow pre-shift overtime handling

#### Rules, warnings, or behavior notes

* overtime requests and payroll overtime amounts depend on these settings
* if overtime thresholds are too low or too high, approved overtime can still produce payroll results the company does not expect
* this page defines the company rule layer; overtime review later happens in **Hours**, **To Do**, and **Pay Check**

#### Image Placeholder

\[Image: Overtime Settings page showing company overtime rules and calculation controls]
