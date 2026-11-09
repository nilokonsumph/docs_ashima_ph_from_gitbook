# import shift assignments

## import shift assignments

use shift import to assign dated employee schedules in bulk from the current Ashima template.

{% hint style="warning" %}
**warning:** a bulk shift assignment can change attendance and payroll for many employees. review the upload results before continuing and recalculate affected open payrolls.
{% endhint %}

\*\*Navigation:\*\*\ go to \*\*Shifts → Shifts Overview\*\*, then select \*\*Import File\*\*.

### how do i import assignments?

1. select **Download Template**. the current page identifies template version `3.2.1` as recommended.
2. complete the employee and shift assignment rows without changing the template columns.
3. save the file in the required CSV format.
4. select the completed file.
5. upload the file.
6. review the status of every row.
7. if Ashima shows warnings, review them before choosing whether to continue.
8. confirm the import only after the displayed record count and messages are correct.
9. download the error text when the page provides it.
10. correct invalid rows and upload again.

### what should i check in the result?

check the displayed record count and every row status. confirm the employee, schedule, covered dates, warning reason, and whether a row replaces an existing assignment. an uploaded filename is not proof that the assignments were saved.

### what happens after import?

after confirmation, valid assignments appear in the employee shift calendar. for every valid employee-date in the file, Ashima clears any existing dated assignment and saves the uploaded schedule as its replacement. if the date previously used only the payroll-group default, the upload creates a dated override. dates outside the confirmed import remain unchanged. the import does not modify the reusable shift template or the payroll-group default.

Ashima recalculates affected timesheets and creates an **Employee Shift Import** entry in **Settings Audit Trail**. a file that fails template or row validation is not confirmed for saving.

### what happens when an uploaded row overlaps an existing shift?

the uploaded schedule replaces the existing dated assignment for the same employee and date. it does not add a second active shift for that employee-date. an uploaded range performs that replacement for each confirmed date in the range.

before confirming, check the employee, schedule name, **Valid From**, and **Valid Until** values. after confirmation, verify the affected calendar dates and timesheets rather than checking only that the file was accepted.

### understand validation, confirmation, and recovery

the current required columns are **Employee Number/ID Number**, **Valid From**, **Valid Until**, and **Schedule Name**. **Employee Name (First Name and Last Name)** is optional. use `Mark as Rest Day` as the schedule name when applicable.

**Upload File** validates and privately stages the file; it does not by itself save assignments. hard errors stop the upload. a warning retains a private, single-use staged file and requires **Continue**. before saving, Ashima revalidates the company, portal, visibility scope, file, and warning state. a confirmed upload cannot be replayed. the limit is 18,250 expanded employee-date records rather than merely CSV rows.

after confirmation, verify the employee calendars and the **Employee Shift Import** entry in **Settings Audit Trail**. correct rejected rows from the downloadable error information. to correct a saved row, assign the intended schedule for the same dates. if the employee should return to the payroll-group default, clear only the dated override with **Delete**, then verify the default schedule is shown.

### related articles

* [assign shifts](assign-shifts.md#page-034-pages-admin-shifts-assign-shifts-md)
* [shift calendar and overview](shift-calendar-and-overview.md#page-033-pages-admin-shifts-shift-calendar-and-overview-md)
* [imports and upload manager](../../settings/platform-controls/use-the-upload-manager.md)
