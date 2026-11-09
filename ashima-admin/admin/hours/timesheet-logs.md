# Timesheet logs

## timesheet logs

Use Timesheet Logs to review how employee time entries were interpreted against the assigned shift, identify attendance issues, recalculate changed records, and download the records included in your review.

**Navigation:**\
go to **Hours → Timesheets**.

### how does ashima create a timesheet?

Ashima captures time logs, but the logs alone do not determine the attendance result. The employee's assigned shift provides the context for each work date.

Ashima compares the captured logs with the shift to determine:

* which work date the logs belong to;
* which punches are expected;
* scheduled and actual hours;
* late, overbreak, and total tardiness;
* undertime and absence;
* whether a required punch is missing;
* whether an additional entry should be treated as an excess log; and
* whether the date is a rest day or holiday.

> \[!NOTE] When a timesheet looks incorrect, review the assigned shift and the captured logs together. Correcting punches alone may not fix a result caused by an incorrect shift assignment.

### what punches does a shift require?

The expected punches depend on the shift settings for that work date.

* A shift without tracked breaks normally expects **Clock In** and **Clock Out**.
* A shift with a tracked lunch normally expects **Clock In**, **Lunch Out**, **Lunch In**, and **Clock Out**.
* A shift with tracked additional breaks also expects the applicable break-out and break-in punches.

If an expected punch is missing, the row can require correction. Ideally, the employee submits a timesheet adjustment. An authorized admin can also correct the record when appropriate.

If more logs are captured than a normal shift expects, an additional entry can appear as an **excess log**. Excess-log handling differs for some rest-day, holiday, flexible-schedule, and open-shift records. Review the shift and day type before removing an entry.

### what do the attendance terms mean?

| term            | simple meaning                                                                       | what to review                                                                    |
| --------------- | ------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------- |
| late            | time recognized after the expected shift start                                       | assigned shift, actual clock-in, and attendance rules                             |
| overbreak       | break time beyond the duration allowed by the shift                                  | break-out and break-in punches and configured break duration                      |
| total tardiness | total tardiness recognized for the day, which can include late and overbreak minutes | detailed late and overbreak values                                                |
| undertime       | scheduled work time not completed before the expected shift end                      | actual clock-out, assigned shift, and approved leave                              |
| absent          | scheduled time with no recognized work or applicable leave coverage                  | schedule, timesheet, and approved leave                                           |
| missing punch   | one or more punches required by the shift are incomplete                             | clock-in, clock-out, lunch, and other tracked breaks                              |
| excess log      | an additional log that does not fit the normal punch structure                       | rest-day, holiday, flexible-schedule, open-shift, or separate-work-period context |

Approved leave can offset tardiness or undertime when it covers the affected part of the shift. Review the attendance result together with the employee's leave records.

### anatomy of a timesheet

Review the fields together rather than reading a punch, color, or total on its own.

| part                         | what it tells you                                     | what to watch for                                                |
| ---------------------------- | ----------------------------------------------------- | ---------------------------------------------------------------- |
| employee and shift date      | identifies the employee and work date                 | overnight work and the correct employee/date                     |
| clock in and clock out       | shows the main work punches                           | a missing clock-out can flag a row even when clock-in exists     |
| lunch and additional breaks  | shows break punches required by the shift             | a blank field matters only when the break is enabled and tracked |
| actual and scheduled hours   | compares recognized work with the schedule            | missing punches, breaks, leave, or an incorrect shift            |
| tardiness                    | shows late, overbreak, and total tardiness            | scheduled start and configured break duration                    |
| undertime and absence        | shows time not covered by recognized work or leave    | shift, leave status, and clock-out                               |
| work schedule                | shows the shift used to interpret the logs            | an incorrect or changed shift can alter the result               |
| source                       | shows where a punch or entry came from                | investigate an unexpected source before editing or deleting      |
| recalculation state          | shows whether the result needs refreshing             | do not rely on a pending result for payroll review               |
| status, approver, and reason | provides adjustment or application context            | resolve pending requests before making a separate correction     |
| location and project         | provides capture or assignment context when available | availability depends on company setup and clock-in method        |

### what do the indicators mean?

The current page uses row and date indicators to highlight conditions such as missing logs, attendance exceptions, changed schedules, employee adjustments, admin/import activity, post-payroll adjustments, rest days, and holidays.

Use the indicator together with the detailed values. An indicator is a prompt to review the row; it does not determine the final attendance or payroll treatment by itself.

### what does the source tell me?

The **Source** helps trace how a punch or timesheet entry entered Ashima. Depending on the record, it can identify desktop, kiosk, mobile, employee, manager, admin/dashboard, imported, or autogenerated activity.

Different punches in one timesheet can have different sources. Review the source beside each punch when investigating a disputed or unexpected entry. Photo, location, and other capture details are available only when supported and enabled for that clock-in method.

### why can an employee clock in before the shift starts?

For a uniform shift, Ashima begins matching the next shift up to two hours before its scheduled start. This helps separate the next shift from work that can still belong to the previous shift.

This is not a universal two-hour rule for every shift type. Overnight, flexible, open-shift, rest-day, and holiday records use their applicable shift and surrounding logs. Review the displayed work date and schedule when a punch appears on a different date than expected.

### why can an employee not punch again immediately?

Ashima rejects another captured employee punch when it occurs less than five minutes after the preceding punch. This helps prevent accidental repeated punches.

This safeguard applies to captured employee punches. Admin add and edit forms use their own validation rules.

### how do timesheets connect to overtime, rest day, and holiday pay?

A captured time log proves that a punch was recorded. It does not always mean that the time is automatically payable.

The usual relationship is:

1. punches are captured;
2. the assigned shift and day type provide context;
3. Ashima identifies the work interval;
4. the employee completes the required overtime, rest-day, or holiday application when approval is enabled;
5. the approver reviews the request; and
6. approved or automatically recognized work becomes eligible for the applicable payroll calculation.

The result depends on employee entitlement, company settings, approval status, and payroll rules.

#### overtime

Ashima compares the requested overtime period with the assigned shift and actual logs. The employee must have a timesheet for the date. The request can also be limited by the overtime grace period, minimum duration, cap, payroll state, and application rules.

Captured time remains reference evidence. Overtime is not payable until the required workflow is completed and approved, unless the applicable setup explicitly permits automatic treatment.

#### rest day and holiday work

Ashima can capture logs on a rest day or holiday. Whether a separate application and approval is required depends on the rest-day, holiday, workflow, entitlement, and payroll settings.

Confirm the day type, employee location, assigned shift, entitlement, and approval state before relying on the payroll result.

> \[!IMPORTANT] **Captured** means the log exists. **Approved** means the required workflow was completed. **Payable** means the approved or automatically recognized work is included under the applicable payroll rules.

### what should i review first?

Prioritize records with:

* missing required punches;
* an attendance warning or changed-schedule indicator;
* actual hours that differ from scheduled hours;
* unexpected tardiness, overbreak, undertime, or absence;
* an excess log;
* a pending adjustment or application;
* an unexpected source;
* a rest-day or holiday date requiring approval; or
* an overnight or cross-date punch under an unexpected work date.

### which settings affect timesheet logs?

| setting or control            | effect on timesheet logs                                                     |
| ----------------------------- | ---------------------------------------------------------------------------- |
| time entry                    | available clock-in methods, photo capture, and entry restrictions            |
| assigned shift                | expected schedule, required punches, breaks, and scheduled hours             |
| tardiness and break settings  | interpretation of late, overbreak, and total tardiness                       |
| overtime settings             | grace period, minimum duration, cap, and application rules                   |
| rest day and holiday settings | whether captured work requires an application and approval before payment    |
| workflow settings             | who reviews applications when approval is required                           |
| leave records                 | whether approved leave covers affected scheduled time                        |
| payroll state                 | whether a direct correction is allowed or a post-payroll process is required |
| access privileges             | whether add, edit, delete, download, or recalculate actions are available    |

Some settings apply company-wide, while others depend on the module, payroll group, shift, location, or employee assignment. When two employees produce different results, compare their assignments and entitlements before treating the difference as an error.

### how do i review an employee's timesheet?

1. Open **Hours → Timesheets**.
2. Search for the employee and select the date or date range.
3. Check whether recalculation is pending.
4. Compare the punches with the displayed work schedule.
5. Confirm which lunch and break punches the shift requires.
6. Review actual and scheduled hours, tardiness, undertime, and absence.
7. Review the indicators, source, status, reason, and approval details.
8. Open the detailed history when you need to trace individual punches.
9. Correct the shift first if the wrong schedule caused the result. Correct the timesheet when the recorded punches are wrong.

### when should i recalculate?

Recalculate when the page shows a pending state after a timesheet, shift, leave, import, or related attendance record was added, edited, deleted, or corrected.

Recalculation interprets the affected logs again using the applicable schedule and rules. If an open pay run already includes those dates, review whether that pay run also requires recalculation.

### how do i download timesheet logs?

1. Apply the employee and date filters required for the review.
2. Select **Download**.
3. Select **Excel** or **CSV**.
4. Open **Advanced Options** when you need to change the timezone. The current default is **GMT +8**.
5. Confirm the download.

The download follows the active view and selected format. The download window shows the number of entries. Large results can be divided into multiple files according to the page's current export limit.

### related articles

* add a timesheet
* edit or delete timesheets
* attendance pages
* punctuality pages
* overtime history
* rest day and holiday work
* time entry settings
* shift settings and assignments
* post-payroll adjustments
