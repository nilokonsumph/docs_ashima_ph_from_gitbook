# configure employee time entry

use employee time entry settings to control how one employee records attendance within the company's available time-entry rules.

**navigation:** open the employee record, then select **Time Entry**.

## what does this page control?

the page provides **Timesheet Required**, desktop and mobile clock-in controls, and employee-level restriction options. When applicable, its employee-specific options include photo capture, individual IP addresses, authentication, and geofencing.

By default, the employee follows the global Time Entry setting. When **Allow Employee Level Restriction** is enabled, the page states that the global setting no longer applies to the covered option and the employee-specific selections take effect. Desktop and Mobile Clock In expose separate employee-level restriction controls.

## which settings control this workflow?

| level            | setting or record                                             | effect                                                                                                                     |
| ---------------- | ------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| company / global | Settings → Hours → Time Entry                                 | supplies the default enabled methods and controls                                                                          |
| module           | Hours settings and approval workflow                          | interprets captured logs and any required approval                                                                         |
| employee         | Timesheet Required; desktop/mobile Employee Level Restriction | determines payroll reliance on actual logs and whether the employee follows global or employee-specific time-entry options |

**Timesheet Required** and clock-in access answer different questions:

| control                                   | what it changes                                                                                                                                      |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Timesheet Required**                    | whether payroll relies on the employee's actual time logs. When it is off, payroll uses the applicable fixed-pay and assigned-earning rules instead. |
| **Desktop Clock In** and its restrictions | whether the employee can use the desktop clock from an allowed network. This is separate from the mobile clock.                                      |

Turning off **Timesheet Required** alone does not turn off desktop clock-in. If the desktop **Employee Level Restriction** is off, the company **Desktop Clock In** setting and trusted-IP rule apply. To turn off desktop clock-in for one employee, enable the desktop **Employee Level Restriction**, turn off **Desktop Clock In**, save, and check the employee's next attempt. Review mobile access separately.

## how do i update an employee setting?

1. open the employee's **Time Entry** page.
2. select the setting you need to change.
3. enable or disable the available option.
4. add or update the required IP or location information.
5. review the effect on employee clock-in and clock-out.
6. click the available save action.

## add or change an allowed IP address

Use **Add Static IP Address** to enter one IPv4 address, an inclusive **From–To** range, or a three-octet subnet. A range allows every address between its endpoints; check the displayed address count before confirming. Location is optional when adding a rule, including when no company location has been configured.

To edit a saved employee IP rule, open its row and complete both the location and description required by the edit form before saving. To remove rules, select only the intended rows and confirm **Delete**. Check the refreshed list afterward.

Correct reversed ranges, non-IPv4 values and overlaps with rules in the same scope before retrying. After saving, verify clock access from the intended network; adding a rule does not change the company-versus-employee restriction switch.

## what happens after saving?

the saved clock-in options govern the employee's next attempt through the affected method. A change to **Timesheet Required** changes payroll's reliance on actual logs; by itself, it does not remove **Desktop Clock In**. Check the saved setting and the employee's next attempt before treating access as changed.

## verify and correct employee time entry

ask the employee to complete a controlled clock action through the intended method, then confirm the source, time, approval state, and shift context in Hours. if the method is unavailable or the log is handled incorrectly, review the company Time Entry setting, employee-level restriction, IP or geofence, device permission, Timesheet Required choice, and employee status before retrying.

## continue in the affected module

* [configure company Hours rules](../../settings/time-entry-hours-shifts-and-holidays/configure-hours-rules.md)
* [review timesheets](../../hours/)
