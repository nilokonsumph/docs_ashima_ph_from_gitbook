# import ingestion entries from CSV

1. open the import page for the intended source record.
2. download the current template.
3. keep these columns: **Employee ID**, **Pay Category**, **Pay Item**, **Date**, **Tax Status**, and **Amount**.
4. use the employee's valid payroll ID and an item available for the selected category and source type.
5. use `mm/dd/YYYY` when the selected item requires a date.
6. enter a non-zero amount and a tax status allowed for the selected item.
7. upload the CSV, review every row error, and correct the file before continuing.
8. use the offered confirmation or save control for the intended valid rows. Check the saved-ingestion list, recalculate the owning record, and review representative employee results.

validation rejects missing required columns, unknown employees, invalid categories or items, invalid dates, zero or missing amounts, and unsupported tax statuses. a successful upload alone does not confirm that rows were saved or complete the owning payroll or payment workflow.

For regular Paycheck **Absent / Absent Adjustment**, the amount must be greater than zero. **Allowance**, **Other Earnings** and **De Minimis** use the active item settings for tax classification; a CSV Tax value cannot override them. Correct missing tax settings before importing. See [add adjustments or ingestion](add-adjustments-or-ingestion.md#which-amount-and-tax-rules-should-i-check) before saving.
