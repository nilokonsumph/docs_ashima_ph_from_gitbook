# recalculate and review retroactive pay

## recalculate and review retroactive pay

Use **Retroactive Pay** when a salary change has an effective date in one or more payroll periods that were already processed. Retroactive pay is generated from the salary and payroll history; it is not entered as a normal recurring earning.

**Navigation:** Go to **Paycheck → Salary Increase and Retro → Retro**.

{% hint style="warning" %}
**Retroactive Pay** must be enabled under **Settings → Paycheck → Earnings → Retroactive Pay**. review the effective date, compensation history, affected closed periods, and existing retro records before generating or recalculating an amount.
{% endhint %}

### what is the retroactive-pay formula?

retroactive pay is incremental. for each affected pay period and supported payroll component, Ashima compares the corrected result with amounts already recognized.

```
new retro due =
recomputed earnings
- original earnings
- prior retro recognized
```

```
total retroactive pay =
sum of the new retro due for all affected pay dates and components
```

**Prior retro recognized** prevents a later salary change from paying the same difference again. if the new retro due is zero, no additional amount is owed for that period and component. do not treat a negative result as an authorized salary recovery unless that workflow is explicitly supported and approved.

### worked example: one affected closed period

```
recomputed earnings = 27,500.00
original earnings = 22,500.00
prior retro recognized = 0.00

new retro due = 27,500.00 - 22,500.00 - 0.00
= 5,000.00
```

### worked example: an earlier retro was already paid

```
recomputed earnings = 25,000.00
original earnings = 20,000.00
prior retro recognized = 3,000.00

new retro due = 25,000.00 - 20,000.00 - 3,000.00
= 2,000.00
```

the new retro is `2,000`, not the full `5,000` difference, because `3,000` was already recognized.

### how does Ashima calculate each affected period?

Ashima evaluates closed payroll periods from the effective date, keeps the applicable salary-rate segments, recomputes supported components, and compares the corrected amount with the recorded original and prior retro amounts. a partial first period covers only eligible time from the effective date onward. later full periods use the applicable full-period basis.

| pay setup                   | regular-pay comparison                                                                                                                        |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **By Month — Semi Monthly** | previous or corrected half-month basis, adjusted for the applicable before/after-effective-date hours or workdays and DIH                     |
| **By Month — Monthly**      | previous or corrected full-month basis, adjusted for the applicable rate segments and DIH                                                     |
| **By Hour**                 | eligible hours before the effective date at the previous hourly rate plus eligible hours from the effective date at the new hourly rate       |
| **By Day**                  | eligible paid days before the effective date at the previous daily rate plus eligible paid days from the effective date at the new daily rate |

### which payroll components can affect the comparison?

The current retro calculation recalculates these rate-sensitive payroll components when the affected closed payroll contains the required source detail:

| component                          | what Retroactive Pay compares                                                                         | what must exist in the source payroll                                                     |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| **Basic Pay or regular pay**       | the recorded result against the result using the corrected basic-pay rate and effective-date segments | the closed payroll period, employee pay type, recorded rate, and applicable days or hours |
| **Absence**                        | the absence deduction at the former rate against the deduction at the applicable corrected rate       | dated absence hours or equivalent payroll detail                                          |
| **Tardiness**                      | the tardiness deduction at the former and corrected hourly basis                                      | dated tardiness minutes or hours                                                          |
| **Undertime**                      | the undertime deduction at the former and corrected hourly basis                                      | dated undertime minutes or hours                                                          |
| **Leave**                          | applicable paid-leave earning or unpaid-leave deduction differences                                   | dated leave detail and the employee's leave treatment                                     |
| **Overtime**                       | overtime rows repriced from the applicable corrected hourly rate                                      | dated overtime hours and the applicable multiplier                                        |
| **Rest day**                       | rest-day rows repriced from the applicable corrected rate                                             | dated rest-day work and the employee's entitlement                                        |
| **Holiday Pay**                    | regular, special, or double-holiday rows repriced under the applicable corrected rate                 | the dated holiday, worked or unworked treatment, and applicable entitlement               |
| **Night Shift Differential (NSD)** | NSD hours repriced from the applicable corrected hourly rate                                          | dated NSD hours and the employee's NSD entitlement                                        |

Yes, **Holiday Pay** and **NSD** can therefore contribute to Retroactive Pay. Their presence is conditional: an employee must have the applicable entitlement and the affected closed payroll must contain the dated holiday or NSD evidence. The same condition applies to overtime and rest-day pay.

The salary-retro calculation does not establish a general recalculation rule for every earning and deduction in payroll. Do not assume that allowances, De Minimis, bonuses, 13th Month, service charge, hazard pay, loans, ordinary deductions, government contributions, or withholding tax are recomputed as component rows unless the displayed Retro breakdown explicitly shows them. Retroactive Pay later enters the receiving payroll as an earning and can affect that payroll's downstream totals under the applicable rules.

Do not add paid leave twice for a monthly-paid employee when it is already covered by basic pay. Post Payroll Adjustment remains a separate correction workflow and should not cause the same component to be paid twice.

### can I run Retroactive Pay more than once for the same employee?

Yes. The current salary-change flow does not impose a one-run limit per employee or closed pay period. A second or third salary change can create additional Retroactive Pay entries when it affects payroll that has already been processed. This is intended for another legitimate effective-dated compensation change; it is not a reason to submit the same change repeatedly.

Before proceeding, compare the new effective date and basic pay with compensation history and the existing Retro list. The same-period warning means another compensation change already falls in that pay-period coverage. Proceeding from the manual Salary Increase form creates a new retro entry; it does not replace or silently merge the earlier record.

### what happens when retro periods overlap?

Ashima reads prior non-voided, non-reversed Retroactive Pay history for each affected closed period and builds an effective-date rate timeline. The new calculation uses the rate already recognized at the new effective date and splits the remaining coverage at later saved change dates. The purpose is to calculate the additional difference from the applicable earlier rate rather than pay the first salary difference again.

Example:

1. a salary change from `40,000` to `45,000` is effective on 1 January and generates Retroactive Pay for a closed January period;
2. a later change to `50,000` is saved with an effective date inside the same January period; and
3. the new Retro calculation should compare the new rate with the rate already established by the earlier change for each applicable date segment. It should not treat `40,000 → 50,000` as wholly unpaid when the `40,000 → 45,000` difference was already recognized.

If two changes use the same effective date, the most recently created non-voided, non-reversed history entry becomes the timeline rate for that date. If a later action is meant to correct an erroneous earlier entry, reverse or correct the earlier record through the supported workflow instead of stacking unexplained entries.

{% hint style="warning" %}
Overlapping coverage can be valid, but it raises the risk of duplicate or contradictory history. Before accepting the new result, expand every affected pay date and reconcile the previous rate, new rate, component differences, prior Retro records, new amount due, and receiving payroll. A warning does not block the manual save. Stop if the new entry repeats the full earlier difference, omits a saved rate segment, produces an unexplained zero or negative result, or cannot be tied to compensation history.
{% endhint %}

### how do i scan for missing retro periods?

use the company scan linked from an individual retro confirmation to find eligible historical periods that still need retro entries. recalculating one retro entry does not automatically run this company scan or generate missing entries.

#### before you scan

confirm that the relevant retro entry is approved. the scan covers records within your authorized company scope.

| date to check                           | limit used by the scan                                                          |
| --------------------------------------- | ------------------------------------------------------------------------------- |
| when the salary adjustment was recorded | June 4, 2026 through the day you run the scan                                   |
| the salary adjustment's effective date  | a rolling six-month limit applies, even when the effective date precedes June 4 |

June 4 is the cutoff for when the adjustment was recorded. it is not the earliest permitted salary effective date.

#### review the preview and generate eligible entries

1. open the individual retro confirmation and follow its company-scan link.
2. run the scan. review the eligible missing periods and any blocked or invalid periods. the preview does not create retro entries.
3. check the complete eligible list before selecting **Generate eligible missing periods**. this action processes eligible missing periods as a batch; it does not offer individual period selection. existing retro entries are skipped rather than duplicated.
4. review the generation results. review blocked or invalid periods individually; they are not generated from the eligible batch.

{% hint style="warning" %}
**before retrying:** if you pause or leave the flow, rescan before generating. if generation is interrupted or the result is uncertain, check the period results and rescan before retrying. some entries may already have been created; do not assume that the batch completed entirely or that nothing was created.
{% endhint %}

### how do I generate retro from compensation history?

1. confirm that the salary increase and effective date are saved in compensation history.
2. open the **Retro** list.
3. select the eligible employee or compensation-history source.
4. generate or preview the retro calculation using the available action.
5. review every affected pay date and component before accepting the result.
6. confirm the open payroll where the approved retro amount will be included, then recalculate that payroll when required.

visible actions depend on the record state and access. paid, reversed, or otherwise ineligible entries cannot be treated like an unpaid draft retro.

### how do I recalculate an eligible retro entry?

use recalculation only for an eligible unpaid entry that has not been reversed.

1. open the **Retro** list and select the entry.
2. use its recalculation action and confirm.
3. review the refreshed summary and each affected pay-date breakdown.
4. verify the payroll that will receive the result.

recalculation refreshes the result from supported current source data. it does not authorize a duplicate payment of previously recognized retro.

### what should I review in the calculation breakdown?

for every affected pay date, verify:

* period from, period to, and pay date;
* previous and corrected salary rates;
* pay-rate type and pay schedule;
* eligible workdays, days, or hours;
* original earnings;
* prior retro recognized;
* recomputed earnings;
* new retro due; and
* component-level differences.

the summary formula, expanded pay-date rows, component totals, and final retro due must reconcile. if a label or displayed component does not reconcile, do not infer the missing amount; preserve the breakdown and escalate it for review.

### where does retroactive pay appear?

when included in payroll, retroactive pay appears as its own earning in Employee Pay Details and the payslip and is included in payroll totals and applicable exports. review the receiving pay date rather than assuming that generating the retro record immediately changes an existing payroll result.

The Retro download supports audit review with fields such as employee, effective date, pay date, period from and to, hours, retroactive pay, generated date, paid date, and source. use the on-screen breakdown for component reconciliation and the download for the cross-period record.

### related articles

* increase an employee's salary
* update salaries in bulk
* review salary increase details
* review employee pay details
* review and recalculate a pay run

### what should i check after a payroll-group transfer?

after an employee moves between payroll groups, review affected historical payroll periods across the relevant groups, including periods outside the current group. a transfer does not mean missing retro entries have been generated automatically.

if an eligible historical period has no retro entry, follow [scan and generate missing retro periods](recalculate-and-review-retroactive-pay.md#scan-and-generate-missing-retro-periods) to review the preview and generation results. the scan is accessed from an individual retro confirmation; this guide link opens the instructions.
