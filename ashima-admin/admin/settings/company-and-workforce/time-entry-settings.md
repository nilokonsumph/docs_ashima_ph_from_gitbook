# Time entry settings

use time entry settings to control how employees clock in and out and which security or location checks are available.

**Navigation:**\
go to **Settings → Hours → Time Entry**.

## what does this page control?

the page controls the company defaults for time entry. On the validated test account, the page includes Kiosk, Desktop Clock In, Mobile, photo capture, company trusted IPs and desktop IP verification, authenticator, mobile-log approval, geolocation fencing, and the minimum interval between punches.

The company page explicitly states that enabled options can then be limited for each employee. An employee uses these global settings unless **Allow Employee Level Restriction** is enabled on that employee's Time Entry page.

## which settings control this workflow?

| level            | setting or record                                 | effect                                                                                                                  |
| ---------------- | ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| company / global | Time Entry Option                                 | defines the default clock-in methods and related security/location controls                                             |
| module           | Hours settings and workflow                       | determines how captured logs are interpreted and whether approval is required                                           |
| employee         | Timesheet Required and Employee Level Restriction | determines whether actual logs are required and whether confirmed employee-specific options replace the global defaults |

Employee-level restriction is a confirmed override for the options named on the employee page. When the restriction is disabled, the global setting is used.

## how do i update time entry options?

1. open **Time Entry**.
2. review the enabled entry methods.
3. enable or disable the applicable options.
4. add or update required IP addresses or kiosk information.
5. review which employees use individual settings.
6. save the change.

## what happens after saving?

future employee time-entry attempts follow the updated company rule. Existing captured logs remain historical records.

## how do i add IP addresses in bulk?

use the IP import page to download the current template, upload the completed file, review validation results, and confirm valid rows.

## related articles

* [employee time entry settings](file:///4659123/workforce/employee_time_entry_settings.md)
* [timesheet logs](file:///4659123/hours/timesheet_logs.md)
* [imports and upload manager](/broken/pages/6c29be8379874ff3086e995775198f2a60d74214)
