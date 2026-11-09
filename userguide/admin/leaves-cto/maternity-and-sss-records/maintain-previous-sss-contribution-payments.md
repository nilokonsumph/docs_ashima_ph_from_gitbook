# maintain previous SSS contribution payments

## maintain previous SSS contribution payments

use this page to maintain previous SSS contribution records, including their remittance dates and official receipt numbers. you can review individual records, update remittance details, download a filtered list, or import contributions for several employees.

**Navigation:** **Leaves → Previous SSS Contribution**.

### find the records you need

1. select an employee from the search suggestions to show that employee's records.
2. choose the contribution month and year. changing either refreshes the list. choose the **Date Filed** newest or oldest order and use the magnifier to apply your search choices.
3. review the employee, contribution month, amount, **Date Remitted**, and **OR #**. use pagination or load more rows to continue through the results.

### how do i maintain a previous contribution record?

#### change one row's remittance details

1. select the pencil beside the intended row.
2. confirm the employee and contribution month, then change **Date Remitted** or **OR #**. the OR field accepts letters, numbers, dashes, slashes, and spaces, up to 50 characters in this form.
3. select the enabled **Update** checkmark to save that row.
4. review the saved values. if the result is uncertain, refresh the list and check the record before entering the change again.

use the row's cancel control to discard the unsaved changes.

#### change several loaded rows

1. select **Edit** at the bottom of the list.
2. change the remittance dates or OR numbers in the rows you need to correct.
3. select **Update**, then review the saved values in each changed row. select **Cancel** to abandon the drafts instead.

{% hint style="info" %}
this edit applies to changed rows currently loaded for editing. it does not update every page matching your filters. if a save fails, refresh and check which values were saved before retrying.
{% endhint %}

### how do i import previous contributions?

select **Upload Previous SSS Contribution**, then download a fresh template. keep all six headers unchanged.

| column                           | what to enter                                                                                               |
| -------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Employee Number**              | the employee's number; required. check it carefully so the contribution belongs to the correct employee.    |
| **SSS Contribution Month (mm)**  | the contribution month as a number from 1 to 12; required.                                                  |
| **SSS Contribution Year (yyyy)** | the four-digit contribution year; required.                                                                 |
| **Total Contributions**          | the contribution amount; required. it must fall within the configured SSS range for that contribution year. |
| **Date Remitted(mm/dd/yyyy)**    | the remittance date in the stated format; optional.                                                         |
| **OR**                           | the official receipt number; optional.                                                                      |

contribution months must fall between the first day of the month 16 months before the upload and the current month, inclusive. for example, an October 2026 upload can contain contribution months from June 2025 through October 2026.

{% hint style="warning" %}
an import can add a contribution or overwrite an existing record for the same employee and contribution month. check the employee, month, amount, and remittance details before confirming an overwrite.
{% endhint %}

1. save the completed file as CSV, no larger than 10 MB.
2. browse for the file and check its name. remove an incorrect selection before choosing the correct file.
3. select **Upload File**. this validates and stages the data; it does not save the contribution records yet.
4. review the **Rows**, **Ready**, and **Errors** totals and each row's details. check which rows are ready to add, which will overwrite existing records, and which have errors. use **Download Errors** when available to review corrections.
5. select **Confirm Import** when at least one valid row exists and you intend to save those valid rows. invalid rows are skipped. select **Cancel** instead to discard the staged file and return to the upload form.
6. wait for the result, then verify the saved contributions in the list. if the staged upload expired or cannot be read, upload the file again and review its preview before confirming.

after a partial import, check the saved list before correcting and uploading failed rows. avoid unintentionally overwriting records that were already imported successfully.

### how do i download the contribution list?

1. apply the employee, month, year, and search filters for the records you need.
2. select **XLS** or **CSV**.
3. if the extra-column form appears, choose the additional fields and select **Continue**. closing that form discards the extra-column selection.
4. check the downloaded file's employees, months, and coverage. the export includes up to 100,000 filtered records; verify coverage if your result is larger.

the download follows the applied list filters and sort order. row checkboxes select records for deletion; they do not limit the download. unapplied search edits do not change the export scope.

### how do i delete an incorrect contribution record?

only authorized users can delete active contribution records.

1. select the intended rows, up to 100 records, then select **Delete**.
2. review the password confirmation. if you need to check the selection, choose **Cancel** and return to the list.
3. enter your Ashima account password and select **delete** to confirm.
4. review the result and refreshed list to confirm which records were removed. if authentication or deletion fails, follow the message and check the saved list before retrying.

### related guidance

* [maternity and SSS records](./)
* [Leaves and CTO](../)
