# Allowances

Use Allowance settings to define a reusable allowance, then assign it to eligible employees through the Earnings allowance page.

**Navigation:**\
for setup, go to **Settings → Paycheck → Earnings → Allowance**.\
for assignment, go to **Earnings → Allowance**, then open the employee.

## what makes an allowance different?

An allowance is a named earning with its own applicability, rate method, payout schedule, and tax rule. Use Other Earnings for an earning that does not need the allowance-specific rate and eligibility behavior. Use De Minimis only when the item should follow the De Minimis ceiling and excess workflow.

## before you begin

* confirm the allowance name and business purpose;
* decide who is eligible by employment type, rank, department, or the displayed supported category;
* decide whether the amount is flat, based on a daily-rate percentage, or based on an hourly-rate percentage;
* decide whether absence or worked-time rules should affect the amount;
* choose the frequency and payroll payout schedule;
* confirm whether it is **Taxable** or **Non Taxable**; and
* check whether an item with the same name or purpose already exists.

Active allowance names must be unique. A new or edited allowance must remain distinguishable from existing payroll history.

## which settings control the allowance?

| level          | setting or record                    | effect                                                                                                    |
| -------------- | ------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| company / item | allowance definition                 | controls name, applicability, rate method, frequency, payout schedule, and tax rule                       |
| employee       | allowance assignment                 | connects the item to one employee and stores the supported employee amount, percentage, dates, and status |
| payroll        | open pay run and recalculation state | determines when the assigned allowance appears in payroll and whether a recalculation is required         |

The company item must be active and the employee assignment must be active before payroll can use it.

## how do i create an allowance?

1. Open **Settings → Paycheck → Earnings → Allowance**.
2. Select **Add Allowance**.
3. Enter a unique allowance name and description.
4. Select **Applicable For** and complete the displayed rank, department, employment-type, or other coverage fields.
5. Choose the allowance rate method:
   * **Flat Rate** for a fixed amount;
   * **Daily Rate Percentage** for a percentage-based daily-rate calculation; or
   * **Hourly Rate Percentage** when that option is available for the selected setup.
6. Complete the absence, hours-worked, or coverage controls shown for that method.
7. Select the frequency. The current workflow supports schedules such as per payroll, per worked day, weekly, twice monthly, monthly, or one time, depending on the item setup.
8. Select the payroll payout schedule, such as every payroll or a specific payroll in the month. Twice-monthly setup requires two payroll selections.
9. Choose the tax rule:
   * **Taxable**; or
   * **Non Taxable**, which the current screen identifies as included in the ₱90,000 exemption-ceiling handling.
10. Review the complete setup, then select **Save**.

## how do absence and proration choices affect the allowance?

The allowance setup can determine whether the item remains payable during absence or is prorated using supported worked-day or worked-hour logic. Read the displayed question carefully: the stored system rule can be expressed as entitlement during absence rather than a simple “prorate yes/no” label.

Before saving, use a representative employee example:

* fully worked period;
* period with absence;
* period shorter than the normal schedule; and
* employee outside the selected applicability group.

## how do i assign an allowance to an employee?

1. Open **Earnings → Allowance**.
2. Search for the employee and open the employee allowance details.
3. Select **Assign Allowance**.
4. Select the allowance item.
5. Confirm the employee-specific amount or percentage and the displayed dates or schedule.
6. Review the tax rule and payout behavior inherited from the item.
7. Save the assignment.
8. Confirm that the assignment appears as active.
9. Recalculate an affected open payroll and review the resulting pay details.

Creating the setting alone does not assign it. Applicability narrows who should receive the item; it does not replace the employee-assignment step.

## one-time, recurring, and multiple allowances

* Use a one-time schedule for a single approved payout.
* Use a recurring schedule when the same item should continue according to its dates and payroll schedule.
* An employee can have different allowance items when each item has a distinct business purpose.
* Before assigning another record for the same allowance, review the employee's active and historical lists. Do not create a second active record merely to correct the first.

## how do i pause, stop, correct, or remove an allowance?

Open the employee allowance detail and use the supported edit, status, cancel, or delete action shown for the record.

* Correct an editable active assignment when the business meaning is unchanged.
* Set the assignment inactive or cancel future use when supported.
* Preserve historical payroll meaning; stopping future use does not rewrite completed payroll.
* If the allowance definition itself should no longer be assigned, update its supported status instead of repurposing its name.

## what happens in payroll?

An active assignment becomes eligible for payroll according to the item's calculation, schedule, dates, and employee applicability. After any change:

1. recalculate the affected open pay run;
2. review the employee pay details and allowance line;
3. confirm taxable/non-taxable treatment and any ceiling effect; and
4. verify the payslip and payroll register presentation.

## warnings and troubleshooting

* **Allowance Name must be unique:** search existing active items and use the intended existing definition or create a clearly different business item.
* **No allowance available to assign:** confirm the item is active and applicable to the employee.
* **Allowance missing from payroll:** check assignment status, dates, payroll schedule, applicability, absence/proration rule, and recalculation state.
* **Unexpected tax result:** review the item's tax rule and cumulative ₱90,000 ceiling treatment; “Non Taxable” is not a promise that every peso remains untaxed in every cumulative scenario.
* Do not delete or rename a used item merely to hide it from future selection.

## related articles

* [earnings items overview](/broken/pages/ba9a223f8ab1205e51114762ade2b8c0417feb55)
* [other earnings](/broken/pages/89f0b1d6a87a6070a5aad8d085d2b7812028be7e)
* [de minimis settings](/broken/pages/469b604113ca86caa86d47b8881d8ba260f6e939)
* [employee pay details](/broken/pages/fcfc361d8c5815ad174e9f207d84d69146e1b6b2)
* [payroll register](/broken/pages/058da055ad563cd1bba818da1baca29f93b8e92f)
