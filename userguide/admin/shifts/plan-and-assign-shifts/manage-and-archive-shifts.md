# manage and archive shifts

## manage and archive shifts

use manage shifts to archive a shift that should no longer appear in active setup or assignment lists, and unarchive it when it is needed again. archiving changes the shift's setup availability; it does not delete historical employee schedules.

{% hint style="warning" %}
**warning:** archiving a shift does not remove historical schedules. a default shift, a shift used by an active payroll group, or a shift whose most recent assignment is still within the protected period cannot normally be selected for archiving.
{% endhint %}

**Navigation:**\
go to **Shifts → Shifts Planning**, then select **Manage Shifts**.

### what does this page display?

the active view lists the shift name, shift type, number of payroll groups using it as a default, and the last-assigned date. select **Archived List** to review archived shifts.

an unavailable checkbox means that the shift is protected from the normal archive action. current rules protect:

* default shifts;
* shifts used by at least one active payroll group; and
* shifts whose latest active employee assignment ends less than six months before today, including a future assignment.

administrative access does not mean that a protected checkbox should be bypassed. remove or finish the related setup dependency through the correct workflow first.

### why should i archive shifts that are no longer used?

new schedules accumulate as working hours, rest days, teams, and arrangements change. if obsolete shifts remain active, the selection lists become longer and administrators can more easily choose the wrong schedule during employee setup, bulk assignment, or import preparation.

review the active shift list regularly and archive schedules that are no longer intended for new assignments. archiving keeps the active list easier to search and use while preserving the shift for history and later restoration.

{% hint style="success" %}
**tip:** include shift cleanup in a regular administrative review, such as quarterly or before a new scheduling cycle. use **Default for Pay Groups** and **Last Assigned** to identify dependencies before archiving.
{% endhint %}

archiving is available only after the shift is no longer protected as a default, an active payroll-group dependency, or a recently assigned schedule. move employees or payroll groups to the intended active schedule first, then archive the old shift when it becomes eligible.

### how do i archive a shift?

1. search for the shift.
2. review **Default for Pay Groups** and **Last Assigned**.
3. select the shift.
4. click **Archive**.
5. review **Are you sure you want to archive selected shift/s?**.
6. confirm the action.

### how do i restore an archived shift?

1. select **Archived List**.
2. search for the shift.
3. select the shift.
4. click **Unarchive**.
5. review **Are you sure you want to unarchive selected shift/s?**.
6. confirm the action.

### what happens after archive or unarchive?

after a successful archive, the shift moves from **Manage Shifts** to **Archived Shifts**, where its **Archive Date** is shown. after a successful unarchive, it returns to the active list and is available for future setup or assignment subject to the normal shift rules.

### delete a shift template

delete a template only when it should not remain available and archive is not the intended maintenance action.

1. open the settings page for the applicable shift family.
2. select the template.
3. select the delete action.
4. review the dependency warning and confirm only when the template is eligible.

a template assigned as a payroll-group default cannot be deleted through the ordinary action. resolve the listed payroll-group dependency first. after deletion, confirm the template is absent from the active settings list. if historical reference or later reuse is required, archive the template instead of deleting it.

### how do shift settings relate to employee schedules?

* shift setup creates a reusable company schedule and shift type.
* payroll groups can select a shift as their default work schedule.
* employee shift assignments apply a reusable schedule to selected employees for dated periods.
* archive controls whether the reusable schedule remains available for active use; it does not erase prior assignments or their history.

changing a default, employee assignment, or dated schedule is a separate action from archiving the reusable shift.

### verify or correct archive status

after archiving, confirm the shift appears under **Archived List** with its archive date. after unarchiving, confirm it appears in the active list and is available for supported future assignment.

if the wrong shift was archived, unarchive it. archiving does not change historical assignments. if a shift cannot be selected, resolve the displayed default, active payroll-group, or recent-assignment dependency instead of bypassing the protected state.

### related articles

* [shift calendar and overview](shift-calendar-and-overview.md#page-033-pages-admin-shifts-shift-calendar-and-overview-md)
* [assign shifts](assign-shifts.md#page-034-pages-admin-shifts-assign-shifts-md)
* [shift settings](../../settings/time-entry-hours-shifts-and-holidays/configure-shift-rules.md)
