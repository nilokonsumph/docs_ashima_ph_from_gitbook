# use post-payroll adjustments

## use post-payroll adjustments

use Post Payroll Adjustment (PPA) for an eligible correction to a previous closed payroll when the original pay run can no longer be changed.

**Navigation:**\
go to **Settings → Pay Run → Post Payroll Adjustment** to review the governing options. Start the eligible correction from its source Hours, Leave, Rest Day, or Overtime workflow.

### post payroll adjustments (PPA)

#### does waiting for approval make a timesheet eligible for PPA?

no. a timesheet tied to payroll **Waiting for approval** is blocked from the normal edit flow. a closed-payroll timesheet edit must pass the PPA settings and date checks. a prior PPA already used for that employee/date can also block another edit. follow the displayed message rather than treating all locked requests as eligible PPA.

for closed-payroll timesheets, the date window depends on the employee's payroll context and the configured lookback. a limit of six is not a guarantee that every date in the preceding six calendar months is eligible. **Excess Hours** included in a closed payroll cannot be edited through this PPA path.

**what are PPAs?**

**post payroll adjustments** carry eligible corrections from a previously closed payroll into a later open payroll. a waiting-for-approval state alone does not establish eligibility.

use PPA when a payroll-affecting update is raised too late for the original open pay run, such as:

* a missing timesheet
* an overtime entry that was not filed in time
* a leave application or time-related correction that affects already-processed payroll

when a late correction is approved through the PPA process, the resulting payroll effect carries into the current open pay run as a post-payroll adjustment. depending on the correction, this carry-over can be either positive or negative.

**what settings control whether PPA is allowed?**

PPA is controlled by company settings. PPA is only available if your company has enabled this function, and only within the allowable past-payroll period set by your company.

these settings determine:

* whether **Post Payroll Adjustment** is enabled at all
* whether employees are allowed to start PPA requests
* how far back a closed payroll date can still be handled through PPA

if the company turns off employee-initiated PPA, employees cannot file PPA requests even if PPA remains available for admins.

**what can PPA cover?**

PPA is used for eligible late payroll corrections after the original payroll is already closed and can no longer be updated through the normal open-payroll flow.

**common PPA coverage includes**:

* missing timesheet correction
* timesheet adjustment
* late overtime application
* late leave application
* open-shift PPA
* payroll effects that can later appear as post-payroll adjustments such as workday, tardiness, undertime, leave, overtime, and night shift differential

not every late request is automatically eligible for PPA. depending on the correction type and date, Ashima can block:

* holiday-related corrections where that workflow prohibits PPA
* shift change adjustments connected to a closed payroll
* items that were already processed as PPA once before

these checks are not identical in every Hours, Leave, Rest Day, Open Shift, or Overtime workflow. follow the message shown where you start the correction instead of applying one workflow's restriction to every PPA request.

**how far back can PPA be used?**

PPA only works within the company's allowed lookback period.

this setting limits how many past payroll periods can still be corrected through PPA. If a date is already outside that allowed range, the system blocks the request for that period.

if no custom company setting has been saved, Ashima uses six previous payroll-calendar dates for the employee's pay schedule. this does not mean six calendar months or six confirmed closed-run records; the request must still pass the applicable date, year-boundary, payroll-state, holiday, freeze, and prior-PPA checks.

**when should I use PPA?**

Use PPA only when a correction is discovered after payroll has already moved forward and the original pay run can no longer be updated through the normal open-pay-run flow. Do not use PPA for corrections that can still be handled within the original open pay run.

**how do Post Payroll Adjustments appear in payroll?**

PPA items appear in payroll detail and payslip output as separate post-payroll adjustment values rather than as standard open-pay-run entries. This keeps them identifiable as corrections to prior payroll periods.

In some payroll displays and exports, certain PPA categories may appear grouped. For example, **Holiday / Rest Day** may appear together rather than as two completely separate lines.

**how does PPA affect payroll?**

approved PPA corrections carry into a later open pay run. the adjustment can be positive or negative, depending on the correction.

1. review the original work dates, hours, request, approval evidence, and the schedule assigned on those dates. eligible Workday and NSD corrections use that historical schedule rather than automatically using the employee's current default shift.
2. confirm that the source pay run is closed when the workflow requires it.
3. complete the PPA approval required by the request's workflow. employee-initiated requests follow approval; admin-initiated corrections are recorded directly, as explained below.
4. recalculate the employee's paycheck in the receiving open pay run.
5. review the adjustment in that paycheck and **Employee Pay Details**.

the request must still pass the applicable PPA settings, date, payroll-status, holiday, freeze, and previous-adjustment checks. the historical-schedule rule above applies to eligible Workday and NSD corrections; it does not extend their rules to every PPA type.

**who can start a PPA?**

PPA can be started by either the employee or the admin, depending on the module and the company settings.

* **Employee-initiated PPA** — the employee files a late correction after the original payroll is closed. This follows the normal approval workflow for that request type and is reviewed in To Do before the payroll effect is carried into a later open pay run.
* **Admin-initiated PPA** — the admin records the correction directly in the admin portal. This appears in history as **admin initiated** and does not require employee-side approval.

**does employee-initiated PPA require approval?**

yes. when the PPA is started by the employee, it follows the normal approval workflow for that request type.

in practice, this means:

* the request is submitted as a PPA request
* approvers review it in **To Do**
* once approved, the payroll effect is carried into a later open pay run

**does admin-initiated PPA require approval?**

no, admin-initiated PPA is recorded directly. it can appear in history as **admin initiated**. this is used when the admin is applying the correction directly instead of waiting for the employee to file it through the employee portal.

***
