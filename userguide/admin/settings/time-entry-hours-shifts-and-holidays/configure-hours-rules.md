# configure Hours rules

## find an Hours setting

use the **Hours** settings group to control the company rules that affect how time entries, tardiness, and overtime are interpreted or processed.

the main pages in this settings group are:

* **Time Entry Option Settings**
* **Tardiness Settings**
* **Overtime Settings**

these settings connect directly to later attendance and payroll work:

1. set the company time-entry capture and control rules.
2. set the tardiness, undertime, and overbreak rules.
3. set the overtime eligibility and threshold rules.
4. Let **Hours**, **To Do**, and **Pay Check** use those rules when logs are reviewed and payroll is calculated.

***

## understand how Hours settings affect captured time

Hours settings define the rule layer behind timekeeping.

these pages do not review attendance transactions one by one. Instead, they define how the system should interpret time entries later. In practice, they control:

* where employees are allowed to log time
* whether kiosk, IP, device, or pin-based controls apply
* whether tardiness logic is enabled
* how grace periods and rounding are applied
* when overtime becomes payable
* whether pre-shift overtime is allowed and whether eligible overtime is capped

That is why changes here can affect attendance interpretation, payroll deductions, and payroll earnings at the same time.

***

## use Time Entry Option Settings

use **Time Entry Option Settings** to maintain the company controls for how employees are allowed to log time.

**navigation:** go to **Settings → Hours → Time Entry Option Settings**

## review saved Time Entry Option Settings records

this page displays the company's time-entry control setup under **time entry option settings**.

the page includes company controls tied to:

* **Clock Guard** behavior
* company-approved **IP addresses**
* company **locations**
* **PIN code** lock behavior
* company **MAC address** or kiosk-related controls where used

## manage Time Entry Option Settings

use this page to:

* review the current clock-in restrictions
* maintain allowed IP addresses and location-linked time-entry points
* review kiosk-related setup where the company uses kiosk time entry
* review whether PIN-based lock behavior is enabled

## apply the Time Entry Option Settings rules

* changes here affect how time logs are accepted before admins ever review them in **Hours**
* location, device, IP, or kiosk restrictions can prevent a time entry from being treated as valid in the intended way
* this page is part of timekeeping control, not payroll calculation directly, but its settings still affect what attendance data payroll later receives

## use Tardiness Settings

use **Tardiness Settings** to define how tardiness, undertime, and overbreak should be evaluated for the company.

**navigation:** go to **Settings → Hours → Tardiness Settings**

## review saved Tardiness Settings records

this page displays the company's tardiness rule setup.

the rule groups include:

* the main **tardiness rule** on or off switch
* **daily grace period**
* **accumulated grace period**
* **tardiness rounding**
* **undertime rounding**
* **overbreak rounding**

## manage Tardiness Settings

use this page to:

* enable or disable company tardiness-rule handling
* define daily or accumulated grace-period behavior
* define rounding intervals for tardiness
* define rounding intervals for undertime
* define rounding intervals for overbreak

## apply the Tardiness Settings rules

* when the main tardiness rule is turned off, the company tardiness option rows are also disabled
* the page validates rounding ranges so the **from** value cannot be greater than or equal to the **to** value
* if daily grace is enabled, the grace minutes and grace start window become required
* if accumulated grace is enabled, the accumulated grace minutes become required
* changing these rules can trigger recalculation work for recent timesheet records because the company timing logic has changed
* these rules affect not only **Tardiness**, but also **Undertime** and **Overbreak** handling in attendance and payroll

## use Overtime Settings

use **Overtime Settings** to define when overtime starts, how much overtime can be counted, and whether special overtime controls apply.

**navigation:** go to **Settings → Hours → Overtime Settings**

## review saved Overtime Settings records

this page displays the company's overtime rule setup.

this setting controls:

* whether overtime settings are enabled
* **overtime grace minutes**
* **minimum overtime minutes**
* whether an **overtime cap** is enabled
* the **overtime cap minutes**
* whether **pre-shift overtime** is enabled

## manage Overtime Settings

use this page to:

* turn overtime-rule handling on or off
* define how many minutes must be reached before overtime is counted
* define the grace minutes around overtime
* cap overtime when company policy requires a maximum
* allow or disallow pre-shift overtime handling

## apply the Overtime Settings rules

* overtime requests and payroll overtime amounts depend on these settings
* if overtime thresholds are too low or too high, approved overtime can still produce payroll results the company does not expect
* this page defines the company rule layer; overtime review later happens in **Hours**, **To Do**, and **Pay Check**

## recover from an incorrect result

verify a representative employee timesheet after saving. if the expected threshold, approval, or payable-time result is wrong, restore the prior rule or correct the affected source record, then recalculate the eligible timesheet and open payroll where required. historical or closed payroll is not corrected merely by changing the setting.

## continue in the affected module

* [review timesheets and Hours results](../../hours/)
