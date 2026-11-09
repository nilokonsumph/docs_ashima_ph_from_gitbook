# assign and manage De Minimis

use De Minimis to assign company-defined De Minimis items to employees, review their calculated non-taxable and excess amounts, and maintain current assignments.

**navigation:** go to **Paycheck → De Minimis** or the current **Earnings → De Minimis** list, then open the employee. Company items are maintained under **Settings → Paycheck → De Minimis**.

## before you assign an item

confirm:

* the correct employee and active De Minimis item;
* the employee matches the item's applicability;
* the eligibility start or waiting period has been met;
* the correct amount or employee-specific value;
* the frequency and payroll schedule; and
* whether the employee already has an active or historical assignment for the same item.

## what does the employee assignment inherit?

the employee assignment uses the company's active item definition, including its De Minimis type, destination, rate method, frequency, and ceiling behavior. Employee-specific fields can provide the supported amount or assignment values, but they do not change the item's business meaning.

## how do i assign a de minimis item?

1. open the De Minimis list.
2. Search for the employee and open the employee detail.
3. select **Assign De Minimis**.
4. select the De Minimis item.
5. review the destination and frequency loaded from the item.
6. enter or confirm the employee amount and other displayed assignment values.
7. review the effective start and payroll schedule.
8. save the assignment.
9. confirm the assignment appears in the employee list.
10. Recalculate the affected open payroll and review the employee pay result.

the workflow accepts non-negative amounts. Use a zero or replacement assignment only when the approved business rule supports it; do not use a negative De Minimis assignment to reverse another payroll item.

## check a new hire’s prorated amount

for a monthly-paid new hire in a semi-monthly period with **Actual Formula** enabled and the applicable days-worked or hours-worked De Minimis method, review the worked days or hours against all scheduled non-rest workdays in the cutoff. paid leave is excluded from this calculation's worked-time basis, and dates before hire are not treated as regular absences. see [new-hire De Minimis proration](configure-de-minimis-item-types-and-limits.md#new-hire-de-minimis-proration) for the complete applicability checklist.

for this same new-hire setup, when the employee does not require timesheets, Ashima uses the assigned De Minimis amount. do not extend this assigned-amount rule to other setups. after recalculating the affected open payroll, review the non-taxable amount and any taxable excess.

## can i assign in bulk?

use the available De Minimis import only with the current matching template and company item names.

1. Download or confirm the current import format.
2. Prepare the employee and item rows.
3. Upload the file through the De Minimis import page.
4. review validation errors and rejected rows.
5. confirm the saved employee assignments in the list.
6. Recalculate and review affected open payroll.

an uploaded file is not proof of a successful assignment. Confirm the row result after processing. The import updates at most one ongoing or paused assignment and keeps completed assignments as history. If it finds more than one mutable assignment or a duplicate completed import state, it rejects the ambiguous row instead of choosing a record to update.

## how do i update, stop, or delete an assignment?

open the employee detail and select the supported edit or delete action.

* use edit for a correction that keeps the same item meaning.
* review effective dates and payroll schedule before changing future use.
* Delete only an eligible assignment and confirm that an open payroll does not rely on the record.
* Completed payroll is not rewritten when a current assignment is removed.

before creating another assignment for the same item, review the employee's current and historical records. Correct an existing editable assignment instead of creating an unintended duplicate.

for a successful deletion through the current flow, the audit snapshot records the employee and assignment reference, setting label, and the assignment's actual amount, rate, frequency, destination, ceiling, excess, start fields, and status. The after-state marks the assignment as deleted by an admin. Missing recorded values appear as **Not set**, rather than being filled from current setting defaults. This describes the current deletion snapshot; it does not add fields to historical audit entries or provide a restoration procedure.

## what should i review in payroll?

* assigned amount;
* calculated non-taxable amount;
* maximum non-taxable amount;
* taxable excess;
* frequency and selected payroll schedule;
* employee eligibility and effective start;
* recalculation state; and
* payslip and payroll-register presentation.

for the current De Minimis proration branch, worked or paid days or hours provide the basis, with at least the expected non-rest scheduled days in the cutoff. When the employee does not require timesheets, the assigned amount is used in this branch.

## warnings and troubleshooting

* **No active item is available:** create or activate the correct company item and confirm applicability.
* **Employee is not eligible:** review rank, department, employment type, and waiting period.
* **Assignment is missing from payroll:** check frequency, payroll schedule, employee payroll group, effective start, and recalculation.
* **Amount is partly taxable:** compare the assignment with the item's maximum non-taxable amount and excess.
* **Duplicate-looking rows:** confirm item, employee, frequency, and effective dates before deleting or adding another assignment.

## continue in the affected module

* [review de minimis in payroll](../../paycheck/)
