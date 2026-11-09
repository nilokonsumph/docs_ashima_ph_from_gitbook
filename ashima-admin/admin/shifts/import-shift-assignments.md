# Import shift assignments

use shift import to assign dated employee schedules in bulk from the current Ashima template.

> \[!WARNING] a bulk shift assignment can change attendance and payroll for many employees. Review the upload results before continuing and recalculate affected open payrolls.

**Navigation:**\
go to **Shifts → Shifts Overview**, then select **Import File**.

## how do i import assignments?

1. select **Download Template**. The current page identifies template version `3.2.1` as recommended.
2. complete the employee and shift assignment rows without changing the template columns.
3. save the file in the required CSV format.
4. select the completed file.
5. upload the file.
6. review the status of every row.
7. if Ashima shows warnings, review them before choosing whether to continue.
8. confirm the import only after the displayed record count and messages are correct.
9. download the error text when the page provides it.
10. correct invalid rows and upload again.

## what should i check in the result?

check the employee reference, shift reference, dates, duplicate rows, and row status. Use a freshly downloaded template so the file matches the current import rules.

the current required columns are **Employee Number/ID Number**, **Schedule Name**, **Valid From**, and **Valid Until**. **Employee Name (First Name and Last Name)** is optional. Use `Mark as Rest Day` as the schedule name when applicable.

## what happens after import?

after confirmation, valid assignments appear in the employee shift calendar. A file that fails template or row validation is not confirmed for saving.

## related articles

* [assign shifts](/broken/pages/8dab2e116e18fe058a546a71372e7b40999f9d9a)
* [shift calendar and overview](/broken/pages/5786b4b9eeb2e11e418af53aa70f4094f7e595d9)
* [imports and upload manager](file:///4659123/settings/imports_and_upload_manager.md)
