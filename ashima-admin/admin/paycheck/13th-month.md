# 13th month

## 13th month

Use 13th Month to prepare, review, recalculate, exclude employees, submit, and produce the available 13th Month payroll outputs.

**Navigation:**\
go to **Paycheck → 13th Month**.

### what makes 13th month different from an ordinary earning?

13th Month is a dedicated payroll process. It is not a reusable allowance or other-earnings item assigned by itself.

The result depends on:

* employee entitlement;
* company 13th Month settings;
* qualifying payroll and payslip values;
* the dates selected for the run;
* exclusions and adjustments;
* future-pay assumptions when the run includes dates without completed payroll; and
* the run's approval state.

### what can i do from the 13th month module?

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

### before you begin

Confirm:

* the intended 13th Month year and selected dates;
* company calculation and proration settings;
* employee entitlement and hire/effective dates;
* closed payroll values available for the covered dates;
* any earlier 13th Month runs or partial releases that the administrator must consider;
* employees who should be excluded from this run; and
* whether future dates require assumptions.

> \[!IMPORTANT] In Ashima, an approved or closed payroll or 13th Month payslip is treated as the completed payroll record. The module does not independently confirm that money was received outside Ashima.

### how is the result calculated?

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

### how do taxable and non-taxable portions work?

13th Month and other benefits use the applicable annual non-taxable threshold. The employee's available threshold space and other covered benefits affect how much of the result is non-taxable or taxable.

Review the split in employee details and the related Year End result. Do not assume the whole amount is non-taxable merely because the employee's 13th Month by itself is below the threshold.

### what are actual and assumed amounts?

* **Actual amounts** come from the applicable completed payroll or payslip records.
* **Assumed amounts** estimate eligible future pay dates that are included before the actual payroll exists.

Assumptions help companies release 13th Month before all December payroll dates have occurred. When assumptions are used, review the result knowing that future attendance or payroll changes are not automatically proof of an adjusted 13th Month payment.

### how do i run 13th month?

1. Open **Paycheck → 13th Month**.
2. Start a run and select the requested year or date coverage.
3. Review the displayed pay dates and run settings.
4. Generate the employee results.
5. Review the employee list and open employees requiring investigation.
6. Apply approved exclusions or supported adjustments.
7. Recalculate the run after any source, exclusion, or adjustment change.
8. Review totals and available outputs.
9. Send a draft or submit for approval according to the company workflow.

### what should i review in employee details?

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

### how do exclusions work?

Use exclusions when an employee should not be included in the current run. Exclusions can be maintained individually or through the available bulk import.

After changing exclusions, recalculate before relying on displayed totals or downloads. An exclusion change can leave the previous amount visible until recalculation is completed.

### when should i recalculate?

Recalculate after:

* including or excluding an employee;
* changing a supported 13th Month adjustment or ingestion;
* correcting an employee's entitlement or source payroll record;
* changing a setting that affects the run; or
* changing the selected coverage while the run remains editable.

Do not rely on an earlier download after recalculation.

### how does 13th month ingestion work?

The current 13th Month ingestion surface supports the 13th Month category and its available withholding-tax entry. Review the employee, amount, run, and downstream tax result before saving.

Use the normal 13th Month run and its employee details for calculation review. Do not use ingestion as a replacement for correcting an incorrect source payroll or setting.

### what should i check before approval?

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

### related articles

* 13th Month settings
* submit, approve, reject, and close payroll
* paycheck adjustments and ingestion
* payslip output
* year end
* termination and final pay
