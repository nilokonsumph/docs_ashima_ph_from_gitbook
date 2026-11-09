# Manage and archive shifts

use manage shifts to archive a shift that should no longer appear in active setup or assignment lists, and unarchive it when it is needed again. Archiving changes the shift's setup availability; it does not delete historical employee schedules.

> \[!WARNING] archiving a shift does not remove historical schedules. A default shift, a shift used by an active payroll group, or a shift whose most recent assignment is still within the protected period cannot normally be selected for archiving.

**Navigation:**\
go to **Shifts → Shifts Planning**, then select **Manage Shifts**.

## what does this page display?

the active view lists the shift name, shift type, number of payroll groups using it as a default, and the last-assigned date. Select **Archived List** to review archived shifts.

an unavailable checkbox means that the shift is protected from the normal archive action. Current rules protect:

* default shifts;
* shifts used by at least one active payroll group; and
* shifts whose latest active employee assignment ends less than six months before today, including a future assignment.

administrative access does not mean that a protected checkbox should be bypassed. Remove or finish the related setup dependency through the correct workflow first.

## how do i archive a shift?

1. search for the shift.
2. review **Default for Pay Groups** and **Last Assigned**.
3. select the shift.
4. click **Archive**.
5. review **Are you sure you want to archive selected shift/s?**.
6. confirm the action.

## how do i restore an archived shift?

1. select **Archived List**.
2. search for the shift.
3. select the shift.
4. click **Unarchive**.
5. review **Are you sure you want to unarchive selected shift/s?**.
6. confirm the action.

## what happens after archive or unarchive?

after a successful archive, the shift moves from **Manage Shifts** to **Archived Shifts**, where its **Archive Date** is shown. After a successful unarchive, it returns to the active list and is available for future setup or assignment subject to the normal shift rules.

## how do shift settings relate to employee schedules?

* shift setup creates a reusable company schedule and shift type.
* payroll groups can select a shift as their default work schedule.
* employee shift assignments apply a reusable schedule to selected employees for dated periods.
* archive controls whether the reusable schedule remains available for active use; it does not erase prior assignments or their history.

changing a default, employee assignment, or dated schedule is a separate action from archiving the reusable shift.

## related articles

* [shift calendar and overview](/broken/pages/5786b4b9eeb2e11e418af53aa70f4094f7e595d9)
* [assign shifts](/broken/pages/8dab2e116e18fe058a546a71372e7b40999f9d9a)
* [shift settings](file:///4659123/settings/shift_settings.md)
