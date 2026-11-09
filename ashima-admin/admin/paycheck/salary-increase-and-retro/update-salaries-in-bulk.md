---
hidden: true
---

# update salaries in bulk

update salaries in bulk

use **Retroactive Pay Import** to upload new basic pay and effective dates for multiple employees in one file.

{% hint style="warning" %}
this import updates employee salary records. download a fresh template, review every effective date, and correct validation errors before you continue.
{% endhint %}

**navigation:**\
open **Retroactive Pay Import** from the import area.

the screen is named **Retroactive Pay Import** because it calculates retroactive pay when an uploaded effective date belongs to a previous payroll period. you can also use it to upload current or future-dated basic pay changes.

### how do i upload salary changes?

1. select **Download Template** to get the latest CSV template.
2. enter one employee salary change per row.
3. remove the sample and empty rows from the file.
4. save the completed file as CSV.
5. select **Browse File** and choose the CSV file.
6. select **Upload File**.
7. review the validation result for every row.
8. select **Retry** to correct the file, or **Continue** to process only the valid rows.

### template fields

* **Employee ID (\*)** — enter the employee ID using the format shown in the downloaded template.
* **New Basic Pay (\*)** — enter the employee's new basic pay as a valid amount.
* **Effective Date (format: "YYYY-MM-DD") (\*)** — enter the first date when the new basic pay applies.
* **Adjustment Details** — enter a short reason or reference for the salary change.

(\*) required fields must be completed for every row.

### what file rules should i follow?

* use the latest downloaded template.
* do not change, add, delete, or rearrange the column headers.
* delete the example rows before uploading.
* delete empty rows.
* upload a CSV file only.
* upload no more than 50 employee records in one file; use another file for additional records.

### what happens when the file has errors?

ashima lists the rows that did not pass validation. select **Retry** if you want to correct and upload the file again.

if the file also contains valid rows, select **Continue** to process the valid rows and ignore the rows with errors. review the result before leaving the page so you know which employees still need correction.

### what happens after the import?

ashima records each valid salary change in the employee's compensation history. the uploaded effective date determines how the change is handled:

* a current-period date is used in the applicable payroll calculation.
* a future date waits until the new basic pay becomes effective.
* a date in a payroll period already processed is handled as retroactive pay when retroactive pay is enabled.

recalculate any affected open pay run, then review the employee's compensation history and payroll result.

### related articles

* salary increase
* increase one employee's salary
* salary increase details
* retroactive pay
