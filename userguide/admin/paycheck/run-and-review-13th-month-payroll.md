# run and review 13th Month payroll

## run and review 13th Month payroll

### 13th month

Use 13th Month to prepare, review, recalculate, exclude employees, submit, and produce the available 13th Month payroll outputs.

**Navigation:**\
go to **Paycheck → Earnings → 13th Month**.

#### what makes 13th month different from an ordinary earning?

13th Month is a dedicated payroll process. It is not a reusable allowance or other-earnings item assigned by itself.

The result depends on:

* employee entitlement;
* company 13th Month settings;
* qualifying payroll and payslip values;
* the dates selected for the run;
* exclusions and adjustments;
* future-pay assumptions when the run includes dates without completed payroll; and
* the run's approval state.

#### what can I do from the 13th month module?

Depending on the run state and your access, the module provides actions to:

* create and review a 13th Month run;
* open employee details;
* recalculate the run;
* include or exclude employees;
* import exclusions;
* add the supported 13th Month ingestion entry;
* send a draft;
* submit the run for approval;
* generate or review 13th Month payslips; and
* download masterlist, ingestion, bank-file, and other available outputs.

#### what does the 13th Month workspace show?

the workspace lists runs in one table. review the **Year**, **Pay Schedule**, covered **Pay Dates**, employee details, **Total**, **Last Recalculated**, **Status**, **Approved Date**, and **Created By**. draft and approved runs can appear in the same workspace; use the status and dates to identify the run you need.

#### before you begin

Confirm:

* the intended 13th Month year and selected dates;
* company calculation and proration settings;
* employee entitlement and hire/effective dates;
* closed payroll values available for the covered dates;
* any earlier 13th Month runs or partial releases that the administrator must consider;
* employees who should be excluded from this run; and
* whether future dates require assumptions.

{% hint style="warning" %}
**important:** In Ashima, an approved or closed payroll or 13th Month payslip is treated as the completed payroll record. The module does not independently confirm that money was received outside Ashima.
{% endhint %}

#### how is the result calculated?

The existing guide uses this core relationship:

```
13th Month = (qualifying earnings - qualifying deductions) / 12
```

The qualifying items depend on company settings. They can include basic pay and other enabled earnings, less enabled absence, tardiness, undertime, or other qualifying deductions. Eligible adjustments and PPA amounts can also affect the result.

For a non-prorated setup, the guide uses:

```
base 13th Month = total qualifying pay for the covered year / 12
```

Example: if total qualifying pay for the covered year is `240,000`, the base result is `240,000 / 12 = 20,000` before applicable adjustments and tax treatment.

For a prorated setup, Ashima calculates the qualifying result for each covered payroll and totals the covered amounts.

Example: if qualifying pay for one covered payroll is `10,800`, that payroll contributes `10,800 / 12 = 900` before the other covered payroll results are added.

Do not compare employees only by salary. Differences can result from hire date, entitlement, selected dates, actual payroll, attendance-based deductions, adjustments, assumptions, and company settings.

#### how do taxable and non-taxable portions work?

13th Month and other benefits use the applicable annual non-taxable threshold. The employee's available threshold space and other covered benefits affect how much of the result is non-taxable or taxable.

Review the split in employee details and the related Year End result. Do not assume the whole amount is non-taxable merely because the employee's 13th Month by itself is below the threshold.

#### what are actual and assumed amounts?

* **Actual amounts** come from the applicable completed payroll or payslip records.
* **Assumed amounts** estimate eligible future pay dates that are included before the actual payroll exists.

Assumptions help companies release 13th Month before all December payroll dates have occurred. When assumptions are used, review the result knowing that future attendance or payroll changes are not automatically proof of an adjusted 13th Month payment.

#### how do I run 13th month?

1. Open **Paycheck → Earnings → 13th Month**.
2. Start a run and select the requested year or date coverage.
3. Review the displayed pay dates and run settings.
4. Generate the employee results.
5. Review the employee list and open employees requiring investigation.
6. Apply approved exclusions or supported adjustments.
7. Recalculate the run after any source, exclusion, or adjustment change.
8. Review totals and available outputs.
9. Send a draft or submit for approval according to the company workflow.

#### what should I review in employee details?

Review:

* covered payroll or pay-date entries;
* actual and assumed portions;
* qualifying earnings and deductions;
* prorated values where enabled;
* adjustments and PPA amounts;
* taxable and non-taxable portions;
* withholding tax where applicable; and
* the final 13th Month amount.

If the result is unexpected, check the employee's entitlement, hire date, covered dates, payroll records, settings, exclusions, and adjustments before changing the final amount.

#### how do exclusions work?

Use the current exclusion import sequence and review every row. Invalid rows can remain excluded while a verified valid subset proceeds only after explicit confirmation; upload alone does not change exclusions.

Use exclusions when an employee should not be included in the current run. Exclusions can be maintained individually or through the available bulk import.

After changing exclusions, recalculate before relying on displayed totals or downloads. An exclusion change can leave the previous amount visible until recalculation is completed.

#### when should I recalculate?

Recalculate after:

* including or excluding an employee;
* changing a supported 13th Month adjustment or ingestion;
* correcting an employee's entitlement or source payroll record;
* changing a setting that affects the run; or
* changing the selected coverage while the run remains editable.

Do not rely on an earlier download after recalculation.

#### how does 13th Month ingestion work?

The in-run 13th Month ingestion form supports the **13th month** category and its **withholding tax** item. It is separate from the bulk **13th Month Adjustment Import** below.

1. Confirm the run, pay date, coverage and preselected employee. In the single-employee form, employee search is disabled.
2. Enter the direct amount for **withholding tax**. This item has no editable tax-rule choice here. **Add more** adds another item row for the same employee; remove unwanted rows before continuing.
3. Select **Review and save** and check each **New/Update** classification, effect and destination. Choose **Back** to correct entries without saving, or **Save entries** to commit them. Correct failed checks and review again.
4. Check the saved entries in **view/manage ingestion**. **import file** opens a separate import destination for the source and employee.
5. Return to the run and recalculate separately. Saving these entries does not automatically recalculate the run; review the employee’s tax result afterward.

Use the normal 13th Month run and its employee details for calculation review. Do not use ingestion as a replacement for correcting an incorrect source payroll or setting.

The **13th Month Adjustment Import** is a separate Upload Manager workflow. Use it when approved employee-specific corrections must be applied in bulk to a 13th Month calculation.

#### where do I upload 13th Month adjustments?

Go to **Settings → Upload Manager → Earnings → 13th Month Adjustment**, subject to the user's current navigation and import privileges.

1. Download the current **13th Month Adjustments Import Template**.
2. Keep all six column headings unchanged and in the same order.
3. Complete no more than 50 data rows in one CSV file.
4. Select the CSV and choose **Upload File**.
5. Review every validation message and the number of valid rows.
6. Choose **Retry** to correct and re-upload the file, or **Continue** to save the valid rows while rows reported with errors are skipped.
7. Open the matching 13th Month run, recalculate it, and verify the employee detail before using a masterlist, payslip, bank file, or approval action.

Uploading performs validation only. The adjustment records are saved after **Continue**.

{% hint style="warning" %}
Do not choose **Continue** merely because the file contains some valid rows. Confirm exactly which rows will be saved and correct all unexplained errors first.
{% endhint %}

#### what does each upload column change?

| template column               | what to enter                                                                          | effect on the 13th Month calculation                                                                                                                     |
| ----------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Employee Number/ID Number** | the employee's exact ID in the current company                                         | selects the employee whose 13th Month result receives the row; an unknown ID cannot be applied                                                           |
| **Pay Out Date**              | the exact payout date of the intended 13th Month run, using the template's date format | matches the adjustment to that run; a different date does not affect the intended run                                                                    |
| **Earnings Adjustments**      | an approved positive correction to qualifying earnings                                 | adds to qualifying earnings before the result is divided by 12                                                                                           |
| **Deductions Adjustments**    | an approved positive correction to qualifying deductions                               | adds to qualifying deductions, reducing the calculation basis before division by 12                                                                      |
| **13th Month Adjustments**    | the approved signed correction to the calculated 13th Month amount                     | adds directly after the earnings-minus-deductions result has been divided by 12; a positive value increases the amount and a negative value decreases it |
| **Notes**                     | a concise business reason or supporting reference                                      | is stored with the adjustment for review; it does not change the arithmetic                                                                              |

At least one of the three amount columns must contain a non-zero adjustment for a meaningful row. Leave an unused amount column blank or zero according to the current template. Do not enter a deduction as a negative number: **Deductions Adjustments** is already subtracted by the calculation.

#### how do the three adjustment amounts work together?

For the imported adjustment portion, Ashima uses this relationship:

```
adjusted calculation basis
= qualifying earnings
+ Earnings Adjustments
- qualifying deductions
- Deductions Adjustments

calculated 13th Month before direct adjustment
= adjusted calculation basis / 12

adjusted 13th Month before tax
= calculated 13th Month before direct adjustment
+ 13th Month Adjustments
```

The taxable and non-taxable split and any applicable withholding tax are evaluated after the adjusted 13th Month amount is produced.

**Worked example**

Suppose an employee has a calculation basis of **PHP 240,000** before the imported row. The uploaded row contains:

* **Earnings Adjustments:** PHP 12,000
* **Deductions Adjustments:** PHP 2,400
* **13th Month Adjustments:** PHP 1,000

```
adjusted calculation basis = 240,000 + 12,000 - 2,400
 = 249,600

calculated amount = 249,600 / 12
 = 20,800

adjusted 13th Month = 20,800 + 1,000
 = 21,800 before applicable tax treatment
```

This distinction matters. Entering PHP 12,000 in **Earnings Adjustments** increases the calculated 13th Month by PHP 1,000 because it is included before division by 12. Entering PHP 12,000 in **13th Month Adjustments** increases the result directly by PHP 12,000.

#### what happens when more than one row matches the employee and payout date?

Ashima totals every active adjustment row that matches the employee and exact payout date:

* all matching **Earnings Adjustments** are added together;
* all matching **Deductions Adjustments** are added together; and
* all matching **13th Month Adjustments** are added together.

Uploading the same row again does not replace the earlier row. It can double the adjustment. Before continuing, check the employee, payout date, three amount columns, and notes for duplicate or overlapping entries.

{% hint style="warning" %}
The current upload workflow does not provide an ordinary replace or delete step on the import screen. If a saved row is wrong or duplicated, preserve the evidence and use the company's authorized correction or support process before recalculating. Do not upload an offsetting row unless that correction has been reviewed and approved.
{% endhint %}

#### how do I verify a saved adjustment?

1. Open the 13th Month run whose payout date exactly matches the uploaded **Pay Out Date**.
2. Recalculate the editable run so it reads the current active adjustment records.
3. Open the affected employee.
4. Expand **13th Month Adjustments** in employee details.
5. Reconcile the displayed totals for **Earning (Adj)**, **Deduction (Adj)**, and **13th Month (Adj)** with the accepted CSV rows.
6. Confirm the calculated 13th Month, taxable and non-taxable portions, withholding tax, and final employee amount.
7. Compare the employee detail with the run total and any regenerated output.

If the uploaded row does not appear, first compare the employee ID and payout date with the run. If the amount is larger than expected, check for more than one matching upload row before changing other payroll inputs.

#### what should I check before approval?

* correct year, dates, and employees;
* entitlement and hire-date limits;
* exclusions and adjustments;
* actual versus assumed portions;
* taxable and non-taxable amounts;
* withholding tax entries;
* run total and employee details;
* masterlist and available output consistency; and
* completed recalculation with no stale result.

If the run is rejected, review the reason, correct the editable source or run information, recalculate, and resubmit.

#### related articles

* 13th Month settings
* submit, approve, reject, and close payroll
* paycheck adjustments and ingestion
* payslip output
* year end
* termination and final pay
