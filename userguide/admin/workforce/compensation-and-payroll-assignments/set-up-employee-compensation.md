# set up employee compensation

use compensation details to maintain the employee's payroll group, pay setup, tax and payment information, and payroll entitlements.

{% hint style="warning" %}
**warning:** compensation changes affect payroll. Make changes before payroll approval and recalculate any affected open pay run.
{% endhint %}

\*\*navigation:\*\* go to \*\*Earnings → Compensation\*\*, search for the employee, then open \*\*Compensation Details\*\*.

## review the employee's payroll setup

the page brings together the employee's payroll group, pay rate, schedule, basic pay, tax status, payment method, bank information, contribution choices, and pay entitlements.

use search when looking for an **Inactive** employee in Compensation. Without search, the list includes **Active**, **Resign**, **Terminated**, **Sabbatical Leave**, and **Sabbatical Force Leave**; search uses **Active** and **Inactive**. **End of Employment** is outside both sets. Clear search to return to the normal list scope. Compensation downloads follow the same list/search filtering, subject to existing access and confidentiality checks.

## how do i update compensation setup?

1. search for the employee.
2. open **Compensation Details**.
3. select the section you need to update.
4. click **Edit** when the section uses edit mode.
5. update the fields.
6. review any warning or effective-date requirement.
7. click **Save**.

## which Night Differential choice should i review?

The employee's compensation record can show **Fixed Schedule** as a Night Differential choice. This uses the shift-restriction rule: review the employee's assigned shift alongside the choice before relying on the payroll result. The separate [Night Differential settings](../../settings/payroll-structure-and-rates/configure-pay-rates-for-workdays-rest-days-holidays-overtime-and-night-differential.md) control the applicable rate and rule setup; selecting a compensation choice does not replace those settings.

If a specific employee record still shows an older selection and needs correction, review that record before changing it. Save the intended choice, then recalculate and compare any affected open payroll. Do not reselect the option across all employees without identifying which records are affected.

## set the employee's withholding tax profile

use the withholding tax section for the employee's tax setup. a correction to one pay run belongs in that run's adjustment workflow instead.

1. select **Edit** and review the employee's tax entitlement and the fixed, EWT and VAT choices offered by the section. EWT means expanded withholding tax.
2. enter a fixed amount when the selected method requires it.
3. if you choose **Custom** for the EWT rate, enter a number from **0 to 100**, with up to **two decimal places**. keep the intended decimal rate; do not round it to a whole percentage merely to enter it.
4. review the entitlement choice: choosing not entitled clears the EWT, VAT and rate fields.
5. select **Update**, correct any validation errors and verify the refreshed values. **Cancel** restores the saved setup.
6. review and recalculate affected eligible open payroll.

## what should i use for a salary increase?

use the salary-increase action when you are increasing basic pay and need Ashima to preserve the old rate, new rate, and effective date. Do not replace that workflow with a direct basic-pay edit.

## what happens after saving?

the employee's current compensation setup updates. When the change affects an open payroll, Paycheck should show that a recalculation is required before approval.

## verify the payroll setup

reopen the employee's **Compensation Details** and confirm payroll group, schedule, pay basis, base pay, statutory choices, bank information, and entitlements. recalculate a representative open payroll and compare the employee detail with the saved setup.

if the result is wrong, correct the owning employee or Settings record, then recalculate the eligible open payroll. do not delete compensation history or add a payroll adjustment merely to conceal an incorrect current setup.

## continue in the affected module

* [configure pay groups](../../settings/payroll-structure-and-rates/configure-pay-schedules-and-payroll-groups.md)
* [review payroll](../../paycheck/)
