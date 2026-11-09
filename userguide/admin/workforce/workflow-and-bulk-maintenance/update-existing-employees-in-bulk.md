# update existing employees in bulk

## updates to the Employee 201 records

## using bulk import to update existing employees

if an uploaded row matches an existing employee, the upload updates that employee record instead of creating a new one. Use this carefully.

when updating existing employees:

* Keep the employee's **Employee ID**, **Email**, and name consistent with what is already in Ashima.
* do not use bulk import to change payroll-sensitive setup without reviewing the impact first.
* confirm there are no open payroll implications before changing Payroll Group, entitlements, contribution settings, or Basic Pay.
* review all validation warnings before continuing - valid rows can still update existing employee information.

## update existing records safely

1. download the current employee import template.
2. keep each employee's matching identifiers consistent with the saved record.
3. change only the supported fields that should be updated.
4. upload the CSV and resolve every row error or warning.
5. continue or save only after confirming which rows match existing employees.
6. reopen representative employees and verify personal, employment, compensation, entitlement, and payroll-group results.

the expected result is an update to matched employee records; unmatched valid rows can follow the creation behavior of the import. if a saved value is wrong, correct the owning employee page or use a corrected supported upload, then recalculate or regenerate affected open work. an upload does not rewrite closed payroll.
