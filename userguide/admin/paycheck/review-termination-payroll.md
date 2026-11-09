# review termination payroll

## review termination payroll

***

Use **Termination** to prepare, review, approve, and retain an employee's final-pay record. The process begins with the employee's termination record and continues through payroll calculation, batching, approval, and final output.

**Navigation:** go to **Workforce → Termination**.

{% hint style="warning" %}
Termination changes an employee's status and can affect final pay, tax, benefits, reports, credentials, and year-end records. Complete the source review and use the supported workflow instead of treating the displayed total as sufficient evidence.
{% endhint %}

### what can I do in the Termination module?

Depending on the record state, company setup, and your access, you can:

* create a termination draft and record the employee's effective last day;
* maintain termination information and supporting documents;
* calculate or review missing and catch-up payslips;
* select the payroll components included in final pay;
* add supported final-pay ingestion entries;
* recalculate and inspect the detailed result;
* review 13th Month, remaining-leave, contribution, and tax values;
* move ready employees into the termination masterlist;
* group one or more employees into a batch;
* submit the batch for approval;
* approve or reject it from **To Do's → Termination**;
* download the available masterlist, ingestion, bank, Form 2316, or payslip output; and
* review completed records in Termination History.

### before you begin

Confirm all of the following:

* the employee and **Effective Last Day** are correct;
* time adjustment, leave, overtime, holiday-pay, PPA, and other pending requests dated on or before the effective last day have been decided;
* completed payroll and any missing periods are known;
* compensation, pay type, pay schedule, assigned shift, and attendance inputs are current;
* remaining-leave treatment and eligible leave balances are correct;
* loans, deductions, contributions, earnings, and benefit assignments have been reviewed;
* 13th Month and annual tax information are available when applicable; and
* the required termination approval workflow and approvers are ready.

Do not create a compensating ingestion simply because a source request is still pending. Resolve or correct the source record first, then recalculate final pay.

### how does the termination workflow progress?

The current workflow separates employee preparation from batch approval:

1. select **New Termination** and choose the employee;
2. enter the **Effective Last Day** to create the draft;
3. review or calculate any **Catching-up Payslips**;
4. complete **Termination Details**;
5. edit the supported final-pay inclusions and exclusions;
6. add required ingestion entries and recalculate;
7. send the employee to the termination masterlist;
8. select one or more ready employees and create a batch;
9. review the batch details and submit it for approval;
10. the assigned approver approves or rejects the batch from **To Do's → Termination**; and
11. review approved output and history.

The list can show states such as **draft**, **pending**, **waiting for approval**, **approved**, **rejected**, and **deleted**. Read the visible status together with the available action. A record with a total can still be a draft.

### how do I start a termination draft?

1. open **Workforce → Termination**.
2. select **New Termination**.
3. search for and select the employee.
4. select **Proceed**.
5. enter the employee's **Effective Last Day**.
6. continue to create the draft and calculate the applicable payroll coverage.

The effective last day is the calculation boundary. Eligible work and payroll evidence after that date must not be included merely because it falls inside a normal payroll cutoff. If Ashima reports that the employee is already terminated, already has an approved termination, or is otherwise ineligible, stop and reconcile the employee's existing record instead of creating a duplicate.

### what belongs in Termination Details?

Review the employee's:

* **Effective Last Day**;
* **Termination Type**;
* clearance document;
* resignation letter;
* termination notice;
* termination reason and internal note; and
* last update and person who updated the record.

These fields explain and support the separation record. They do not replace the calculation review on the **Final Pay** tab.

### what are catching-up payslips?

Catching-up payslips represent payroll periods that must be calculated or reviewed before the employee's final pay is completed. Use them when an eligible period through the effective last day is not already represented by completed payroll.

For every caught-up period, confirm:

* pay date and period coverage;
* that the period falls within the employee's employment dates;
* time, leave, overtime, holiday, premium, and pay-item evidence;
* that the amount was not already paid through another payroll; and
* the resulting catch-up net amount.

Catch-up approval and final-pay approval are separate review points. Complete any required catch-up-payslip approval before relying on the final-pay batch.

### how do I review catch-up payslip adjustments?

Use the available catch-up or draft-payslip detail to check **Post Payroll Adjustments** (PPA).

1. choose the caught-up payslip.
2. inspect **Post Payroll Adjustments** and its breakdown.
3. select **Edit** only when the control is enabled.
4. choose whether to include PPA, then select **Save**.
5. review the recalculated data returned by the save flow.

PPA is included by default. Clearing its inclusion removes the non-overtime PPA aggregate; the separate **Overtime** category is not removed by that choice. The selection applies to the payslip being reviewed. Submitted or read-only stages do not provide the same edit access.

### what can be included in final pay?

The **Final Pay** detail can expose the following components when the employee has applicable data:

| group                 | supported components to review                                                                                          |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| current-period pay    | regular hours or basic pay, hours worked, absence, tardiness, undertime, and paid or unpaid leave                       |
| leave and premium pay | remaining-leave conversion, overtime, rest day or holiday pay, and night shift differential                             |
| other earnings        | retroactive pay, PPA, allowances, De Minimis, other earnings, 13th Month, catch-up payslips, and earning-side ingestion |
| deductions            | withholding tax, SSS, HDMF, PhilHealth, insurance, loans, other deductions, and deduction-side ingestion                |
| annual tax            | net taxable pay, tax withheld for the year, tax due, tax refund or payable, and tax status                              |

The page shows only components supported by the employee's records and the current calculation. A `0.00` amount does not by itself prove that the employee lacks the assignment or source record.

### how is final pay calculated?

The current final-pay summary follows this displayed relationship:

```
final pay = total selected earnings - total selected deductions + selected catch-up payslip amounts
```

**Total selected earnings** is built from eligible final-period payroll and the enabled earning components. **Total selected deductions** is built from enabled tax, contribution, loan, deduction, and deduction-ingestion components. Catch-up payslips are added separately in the final-pay total.

This formula explains the summary, but each component still follows its own payroll rule. For example:

* regular pay stops at the **Effective Last Day** and uses the employee's pay type, applicable rate, schedule, eligible days or hours, and paid-leave treatment;
* absences, tardiness, and undertime use the applicable dated payroll evidence;
* overtime, rest day or holiday work, and night shift differential use their eligible hours and configured rates;
* remaining leave uses the supported termination-monetization treatment and available balance;
* 13th Month uses the applicable covered payroll, entitlement, dates, settings, and previous releases;
* contributions, loans, and other deductions use the applicable employee records and final-pay inclusion choices; and
* ingestion changes the matching earning, deduction, contribution, or tax line according to its category.

Do not reproduce a final-pay amount using only monthly salary and the effective last day. The displayed result can also contain catch-up payroll, leave conversion, premiums, assigned items, deductions, annualized tax, and ingestion.

### how do inclusion controls affect the result?

Select **Edit** on the **Final Pay** page to review the available checkboxes and item exclusions. A selected component is eligible to contribute to the recalculated result; clearing a supported item excludes it from this termination calculation.

Some categories also allow individual assigned items or catch-up payslips to be excluded. Review the detail rows before clearing an entire category. After editing:

1. select **Save**;
2. allow Ashima to recalculate;
3. confirm the refreshed component totals; and
4. verify **Total Earnings**, **Total Deductions**, catch-up totals, and final pay.

An inclusion choice does not delete the underlying source record. It controls its supported use in the current termination result.

### how do remaining leave and 13th Month affect final pay?

**Remaining Leave** shows eligible unused leave converted under the supported termination rule. Verify the leave type, remaining units or hours, applicable conversion rate, and resulting amount. A displayed balance is not automatically payable unless that leave type and record qualify for termination conversion.

**13th Month** contributes the employee's applicable termination-period result. Review employment coverage, completed payroll, prior 13th Month releases, company settings, qualifying earnings and deductions, and any supported adjustment. Do not add a full-year amount simply because the employee has a salary record.

### how does final-pay ingestion work?

Use **Ingestion** for an authorized final-pay entry that the termination workflow supports. Categories can cover time and leave, overtime and premiums, allowances, De Minimis, other earnings, deductions, loans, contributions, withholding tax, and 13th Month-related values.

For each entry, confirm:

* the employee and termination record;
* the category and item;
* whether the sign adds to or reduces the result;
* the amount and business basis;
* whether an existing source component already contains the value; and
* where it appears in the final-pay detail and download.

After finishing ingestion, return to **Final Pay** and recalculate. Ingestion is an input; saving it does not prove that the final-pay total has refreshed.

{% hint style="warning" %}
Positive SSS, PhilHealth, or HDMF contribution ingestion must be counted once. After recalculation, confirm that it is not represented in both a base contribution subtotal and an ingestion subtotal. Keep final-pay contribution inclusion separate from catch-up-payslip contribution accounting.
{% endhint %}

### how do i read final-pay and catch-up withholding tax?

Check the tax method saved with the final-pay result before reading the breakdown.

| result                           | what to check                                                                                                                                                                                                           |
| -------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Final-pay withholding tax**    | The tax applied to final pay. For expanded withholding tax (EWT), review the rate or fixed override, eligible earnings and base, VAT base adjustment, signed ingestion and any applicable payroll tax adjustment shown. |
| **Catch-up withholding tax**     | Tax already deducted from the catch-up payslips’ net pay. It is shown separately and is not deducted again from final pay.                                                                                              |
| catch-up tax is zero or negative | Keep the saved value when reconciling the result; a negative amount must not be treated as zero.                                                                                                                        |
| **Not available**                | There is no valid saved catch-up tax value to show. This does not mean zero.                                                                                                                                            |

If withholding is excluded, final-pay tax is zero and its ingestion adjustment is not applied, even if reference base or rate values remain visible. EWT does not use the compensation annualization action.

If an EWT draft cannot recalculate because a rate is missing or invalid, correct its tax setup first. A custom rate must be numeric from 0 to 100 unless the supported fixed override applies. Retry recalculation and inspect the returned result before submitting the final pay.

### how does tax annualization affect final pay?

The **Tax Refund/Payable (Annualization)** section can show:

* **Net Taxable**;
* **Tax Withheld for the year**, including applicable withholding-tax ingestion;
* **Tax Due**;
* **Tax Refund/Payable For The Year**; and
* **Tax Status**.

For compensation withholding, when editing is allowed, the annualization toggle enables or disables the annualization component for this termination. When it is disabled, withholding-tax ingestion is not applied. Review the confirmation, save, and recalculate. If a pre-termination Year End breakdown is available, open it to reconcile the annual totals. When annualization is disabled, the page identifies that state; do not read faded annualization values as an active calculation.

### when must I recalculate?

Recalculate after changing any of the following while the record remains editable:

* final-pay inclusion or item exclusion;
* ingestion;
* termination detail or effective-last-day source information;
* catch-up payroll;
* attendance, leave, PPA, or premium evidence;
* compensation or assigned earning/deduction information; or
* an applicable tax or 13th Month input.

Use the **last recalculation** time and administrator shown on the page. A saved source change that is newer than the last successful recalculation means the displayed total may be stale.

If recalculation returns an error, read the message. When no specific message is supplied, the page shows a retry instruction. Do not proceed to the masterlist until recalculation succeeds and the refreshed detail reconciles.

### what should I review before sending an employee to the masterlist?

Confirm:

* employee, termination type, and effective last day;
* all required catch-up payslips and their approval state;
* current-period pay through the effective last day;
* selected earnings, deductions, and individual exclusions;
* remaining-leave and 13th Month amounts;
* ingestion and contribution treatment;
* annualized-tax status and result;
* total earnings, total deductions, catch-up total, and final pay; and
* a successful, current recalculation.

The page warns when there are unsaved edits or recalculation is required. Resolve those warnings before selecting the action that sends the employee to the masterlist.

### how do batching and approval work?

The termination masterlist holds employees whose individual drafts are ready for consolidated review.

1. open the draft masterlist.
2. compare each employee's **Effective Last Day**, **13th Month Pay**, **Leave Conversion**, **Tax Due**, **Final Pay**, and status with the employee detail.
3. select one or more ready employees.
4. submit the selection to create a batch.
5. open the batch and review its employees and totals.
6. submit the batch for approval.
7. the assigned approver opens **To Do's → Termination**, reviews the batch, and selects **approve** or **reject**.

Batching groups records for review; it does not itself approve the employees. The current approval and rejection confirmations do not provide a reason field. Record any required business explanation through the company's supported review process before taking the action.

### what happens after approval or rejection?

Approval changes the eligible termination batch to approved and makes the supported final outputs available according to company configuration.

Rejection returns the batch to a rejected state. From the termination list or masterlist, use the available **rejected - reuse draft** or move-to-draft action, correct the source or calculation, recalculate, rebuild the batch when required, and resubmit. Do not assume that rejection automatically corrects or recalculates employee values.

### what downloads and records should I reconcile?

Depending on state and configuration, the module exposes termination-list or masterlist downloads, ingestion output, a bank file, termination payslip PDF, Form 2316, and history views. Compare the employee and batch totals with the approved final-pay detail before using an output.

Use **Termination History** for completed batches and historical detail. Treat an approved historical result as a payroll record. Use only the supported correction or move-to-draft behavior shown for its current state; do not silently edit historical values.

### what should I check before completing the review?

* the calculation stops at the correct effective last day;
* no payroll period or component is paid twice;
* selected components match the intended final-pay policy;
* catch-up, remaining-leave, 13th Month, and annualized-tax details reconcile;
* ingestion appears once in the correct category;
* the last recalculation is successful and current;
* the employee detail, masterlist, batch, payslip, bank file, and other downloads agree; and
* the batch status matches the approval decision.

### related articles

* review 13th Month, Year End, and termination approvals
* paycheck adjustments and ingestion
* post-payroll adjustments
* 13th Month
* Year End
* payslip output

### how do i check the printed Final Payslip?

review the saved final-pay details, then open the printed **Final Payslip** and compare the amounts.

* check the final-pay itemization, including retroactive pay and De Minimis lines when those amounts are present.
* check catch-up payroll separately. each catch-up period is shown as a consolidated net amount; its individual earning and deduction lines are not part of the final-pay-only itemization.
* compare each catch-up period with the saved final-pay details.

if an expected amount is missing, review the affected employee's record and payroll period. printing the payslip does not correct a missing underlying amount.
