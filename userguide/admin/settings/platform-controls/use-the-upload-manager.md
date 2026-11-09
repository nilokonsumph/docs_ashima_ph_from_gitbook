# use the Upload Manager

use imports and Upload Manager to create or update supported records in bulk with the current Ashima template.

{% hint style="warning" %}
**warning:** an import may update many employee or payroll records. Use only the current template, review every validation result, and confirm the company and period before saving.
{% endhint %}

\*\*navigation:\*\* go to \*\*Settings → Upload Manager\*\* and select the required import.

## what is the standard import process?

Bank Info is available in Upload Manager to users with the required employee basic-pay privilege.

1. open the required import page.
2. click **Download Template**.
3. complete the file without changing the column structure.
4. save it in the required CSV format.
5. select and upload the file.
6. review every row status and error.
7. download the error file when available.
8. correct invalid rows and upload again, or confirm valid rows.

for Bank Info imports, Ashima rejects duplicate employee IDs, duplicate bank accounts within the file, and an account already assigned to another employee.

## use Payroll WT Adjustment Import

use the current template for an Open or Rejected cutoff. Upload CSV only, up to 2 MB; every row is validated. Review the result, then select **Continue** to save.

## use WT Fixed Import

use the current template for an active draft pay run to set or revert fixed withholding tax. Upload CSV only, up to 2 MB; every row is validated. Review the result, then select **Continue** to save.

## how do i import 13th Month Adjustments?

1. open **13th Month Adjustment** in Upload Manager and download the current template.
2. save the completed file as CSV and upload no more than 2 MB or 1,000 rows.
3. review the required identifiers, date, adjustment, and each validation result.
4. confirm the import to save valid rows; invalid rows are skipped and remain in the displayed result for review.

### which amounts can i enter in a 13th Month adjustment file?

| column                     | accepted amount                                              |
| -------------------------- | ------------------------------------------------------------ |
| **13th Month Adjustment**  | a positive or negative number, but not zero                  |
| **Earnings Adjustments**   | zero or a positive number; negative amounts are not accepted |
| **Deductions Adjustments** | zero or a positive number; negative amounts are not accepted |

check each column separately before confirming the import. the signed-value rule for **13th Month Adjustment** does not apply to the separate earnings and deductions columns.

## what should i check before confirming?

check employee identifiers, dates, amounts, item references, duplicate rows, and the company or payroll period. A successful file upload does not mean every row passed validation.

## what happens after confirmation?

valid rows are saved to the selected module. Invalid rows are not saved and remain available for correction through the displayed result or error file.

## continue in the affected module

* [review imported payroll inputs](../../paycheck/)
