# Paycheck adjustments and ingestion

use **paycheck adjustment** to add a correction directly to an open pay run when the change should not be made through the employee's normal setup or the original Hours, Leave, Earnings, Deduction, Loan, Contribution, or Tax workflow.

> \[!WARNING] a paycheck adjustment changes the payroll being reviewed. Confirm the employee, payroll dates, item, sign, and amount before saving, then recalculate and review the employee result.

**Navigation:**\
go to **Paycheck → Pay Run → Payroll**, open the payroll masterlist, then select **paycheck adjustment**. From Employee Pay Details, the page can also be opened for one employee.

## what does the page display?

the page shows the pay date and coverage dates, then one or more entry rows. Each row can include:

* employee and payroll group;
* pay category and pay item;
* date;
* current rate, new rate, rate percentage, or custom amount;
* total hours; and
* amount.

the available fields change with the selected category and item. Do not assume that every item accepts the same combination of date, hours, rate, or amount.

## which pay categories are available?

the current Paycheck form provides categories for work day, overtime, holiday, night shift differential, leaves, absence, tardiness, undertime, allowance, other earnings, other deductions, loans, contributions, and withholding tax. The pay-item list changes after the category is selected.

## how do i add an entry?

1. verify the pay date and coverage dates.
2. select the employee when the page was not opened from Employee Pay Details.
3. select the pay category and pay item.
4. complete only the fields required by that item.
5. use **preview** to review the calculated result when available.
6. click **save** and review the confirmation.
7. return to payroll review and recalculate as required.

use **add more** when separate entries are required. A separate row is not proof that the entries have different downstream effects; review each item individually.

## how do i review, edit, or delete saved ingestion?

select **view/manage ingestion**. The list shows employee, category, item, date, hourly rate, hours, tax rule, and amount when applicable. Select a saved row before using **edit** or **delete**.

deleting removes the selected saved entry from the current payroll. Recalculate and review the employee and masterlist totals afterward.

## how does file import relate to manual entry?

**import file** opens the import workflow for the same payroll context. Use the current template from that workflow. Before saving an upload, validate employee identifiers, categories, items, dates, signs, and amounts against the manual-entry rules.

manual and imported entries should be reviewed in the same saved-ingestion list and in the resulting Employee Pay Details. Do not assume an uploaded row was accepted only because the file was submitted.

## rules and warnings

* use the original operational module when the source record itself is wrong; use a direct Paycheck entry only for an approved payroll correction.
* a positive or negative value can have a different meaning by item. Confirm whether it increases earnings, increases a deduction, or reverses a prior amount.
* the reviewed form initially displayed the current date even though it fell outside the older payroll coverage. Always verify the date before saving.
* a saved entry can be grouped under **Adjustment**, **Ingestion**, a deduction, a contribution, or a tax line in Employee Pay Details and the payslip.
* source behavior for duplicates is item-specific. Review existing saved rows before adding another entry for the same employee, item, date, and pay run.

## related articles

* [employee pay details](/broken/pages/fc19fcc831aa20c240ee9f0cde597b7cb8a4c2ea)
* [review and recalculate a pay run](/broken/pages/4b2260817fafa8f67821e1a140643d4dd7a297ab)
* [payroll masterlist and readiness](/broken/pages/90993c9dd2e7045a5799c0b820706e27adc169e8)
