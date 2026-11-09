# Withholding tax projection tool

The withholding tax tool (WTT) helps you project each employee’s year-end withholding tax to ensure accurate personal income tax deductions.

Using an averaging formula, the tool estimates total taxable income for the year — helping you identify whether an employee is over-withheld (refund) or under-withheld (payable), so you can take action early.

This feature enhances Ashima’s End-of-Year (EOY) module, providing:

* A real-time snapshot of each employee’s withholding tax position
* Instant identification of refunds or payables
* The ability to make tax adjustments through an open pay run or bulk upload

#### how the projection works

The tool averages the net taxable income from all closed payrolls to date, then applies this average to remaining payrolls for the rest of the year.

It combines both to project each employee’s annual taxable income and corresponding projected WTT.

Best Results Are Achieved When:

* Employees’ taxable allowances or income are recurring.
* All payroll records for the year are recorded in ashima.
* For mid-year joiners, upload the employee’s previous employer Form 2316 to ensure an accurate projection.
* The WT Tool works best when used together with the 13th Month Automation Tool.

### Step-by-Step Guide

#### <sup>Step 1: Access the WT Projection Tool</sup>

1. Login to your ashima admin account.
2.  Navigate to:

    Utilities → Tools → Non-Taxable 90K → WT Tools

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-21 at 5.11.39 PM.png" alt=""><figcaption></figcaption></figure>

#### <sup>Step 2: Review Withholding Tax Projection Details</sup>

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-21 at 5.10.06 PM.png" alt=""><figcaption></figcaption></figure>

Once opened, the WT Projection Tool displays a table listing all employees with the following key fields:\
\
**1. Net Taxable (Current)**

Displays the total taxable pay (e.g., basic pay, OT, holiday pay, rest day pay, allowance taxble, other earnings taxable, etc) from closed payrolls in Ashima.<br>

**2. Tax Withheld (Current)**

Shows total taxes already withheld based on closed payrolls.

**3. Net Taxable (Projected)**

An estimate of the employee’s total taxable income for the year, combining actual income to date with a projection for the remaining payrolls.

{% hint style="info" %}
For _mid-year joiners_, if the previous employer’s Form 2316 is not uploaded to ashima, the projection will be incomplete.

The system will only base calculations on ashima payroll records.
{% endhint %}

**4. Tax Due (Projected)**<br>

Estimated annual tax due using the BIR Annual Tax Table, applied to the _Net Taxable Projected Income_.

**5. 13th Month Pay**

In general, 13th month pay is non-taxable if the total amount does not exceed ₱90,000 in a year. Any amount beyond the ₱90K threshold becomes taxable and is automatically included in the projection.

{% hint style="info" %}
In ashima, you have the option to automate the ₱90K threshold.\
\
When this automation is enabled, ashima automatically creates a ₱90,000 non-taxable bucket.

All non-taxable allowances, other earnings, and any portions of the 13th month pay released throughout the year are added to this bucket to ensure full utilization of the ₱90K benefit.

The system monitors and tracks the total in real time, once the ₱90,000 limit is reached, any amount exceeding the threshold is automatically taxed in subsequent payrolls.\
\
If the 90K Non-Taxable Automation is disabled, 13th month pay will be treated as non-taxable and excluded from projections.\
\
Enabling the ₱90K automation ensures the WT projection reflects your employees’ true taxable position - minimizing year-end corrections.
{% endhint %}

If the ₱90K Non-Taxable Automation is disabled,

_The 13th month pay is treated as fully non-taxable and excluded from the WT projection._<br>

If the ₱90K Automation is enabled,

_You can adjust the percentage of the 13th month already released (e.g., 50%) so only the remaining taxable balance is included in the projection._\
\
To adjust:

Click “Adjust 13th Month”, then enter the percentage released.

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 2.28.35 AM.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Tip: Adjusting the 13th month allows the tool to more accurately estimate each employee’s _total taxable income_ by year-end.<br>
{% endhint %}

To view more detailed information for any employee, simply click anywhere on their row in the table.

This will display a detailed breakdown showing:

* Current and projected taxable income and their corresponding withholding taxes
* Number of payroll periods completed and remaining

Use this view to quickly assess each employee’s year-to-date position and make more informed adjustment decisions.<br>

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 2.36.58 AM.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
To view more detailed information for any employee, simply click anywhere on their row in the table. This will expand the view and display the full breakdown of that employees details.
{% endhint %}

#### <sup>Step 3: Understand the Tax Gap</sup>

The Tax Gap shows the difference between the Projected Tax Due and the Taxes Already Withheld.

This value is based on a system-generated projection, which uses the employee’s historical payroll data and average taxable income to estimate their year-end tax position.<br>

**How to Interpret the Tax Gap:**

*   🟢 Positive Value (Green): Projected or Possible Payable

    Indicates that the projection shows the employee may owe additional tax by year-end.

    → Review the projection carefully and consider increasing WTT in upcoming payrolls to minimize the gap.
*   🔴 Negative Value (Red): Projected or Possible Refund

    Indicates that the projection shows the employee may have overpaid tax to date.

    → Review the current tax deductions and consider reducing or pausing WTT in future payrolls to correct the over-withholding.

Regularly monitoring the Tax Gap helps ensure employees are neither over- nor under-taxed, allowing for smoother year-end reconciliation and avoiding large adjustments later.

{% hint style="info" %}
Important: Because this is a projection, it should be used as a guide — always review it alongside your internal knowledge of each employee’s remaining taxable income, upcoming bonuses, or changes in pay that may affect accuracy.
{% endhint %}

#### <sup>Step 4: Tax Gap Adjustment</sup>

If, after reviewing the projection, you prefer to apply a different withholding tax amount rather than the tax gap suggested by the system - you can use the _Tax Gap Adjustment_ function.

Click on the icon beside the tax gap adjustment amount and a form allowing you to enter any custom amount.<br>

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 2.56.42 AM.png" alt=""><figcaption></figcaption></figure>

This feature allows you to manually adjust the withholding tax based on your own internal calculations or judgment.

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 2.56.29 AM.png" alt=""><figcaption></figcaption></figure>

The Tax Gap Adjustment does not overwrite the projected tax gap — instead, it functions as a plus/minus (_±)_ modifier to fine-tune the system’s calculation.

Any value entered in this field will add to or subtract from the projected tax gap, depending on the employee’s situation.

*   🟢 For Payables (Positive Tax Gap):

    \
    Entering a positive value will add to the existing tax gap, thereby increasing the recommended amount to be withheld.\
    \
    Entering a negative value will reduce the existing tax gap, thereby decreasing the recommended amount to be withheld.<br>
*   🔴 For Refunds (Negative Tax Gap):<br>

    Entering a positive value will reduce the negative amount.<br>

    In most cases this is used to enter a value that brings the total tax gap to zero means the employee will no longer be taxed in upcoming payrolls.

{% hint style="info" %}
Important: Use the Tax Gap Adjustment after carefully reviewing both the projected results and your internal payroll data to ensure any manual changes align with actual taxable income expectations.
{% endhint %}

#### <sup>Step 5: Recommended Adjustment per Remaining Pay Period</sup>

the tool automatically figures out how to spread your tax gap evenly across the remaining payroll periods for the year - so you can see how much to adjust each run.

{% hint style="info" %}
Formula:\
(Tax Gap + Tax Gap Adjustment) ÷ Remaining Pay Periods<br>
{% endhint %}

Use this to guide your adjustments — either manually or through automated uploads.\
\
\&#xNAN;_Note: If you’d like to tweak the recommended adjustment, you’ll need to update the tax gap - there’s no direct way to edit the recommended adjustment itself._

_Use the ± Tax Gap Adjustment function (as explained above) to increase or decrease the total tax gap._

Once updated, the recommended adjustment will automatically recalculate based on the formula.<br>

#### <sup>Step 6: Apply Adjustments</sup>

You have two options to implement WTT adjustments:

**Option 1: Bulk Upload**<br>

1. Download the Withholding Tax Bulk Upload Template (Excel format).
2. Fill in:
   * Employee ID
   * Pay Date
   * WT Amount to be adjusted
3. Upload the completed file to Ashima.

**Option 2: Apply Adjustments via WT Projection Tool**\
\
You can also apply your withholding tax (WTT) adjustments directly within the WT Projection Tool, without needing to prepare a bulk upload file.<br>

1. Select the employees you wish to adjust from the WT Projection table.
2.  Click “Bulk WTT Adjustment.”

    → This action will transfer your selection from the projection view to an existing open pay run, where the adjustments will be processed.<br>

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 3.30.51 AM.png" alt=""><figcaption></figcaption></figure>

3. Specify the pay date of the open pay run where the adjustments will be applied.

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 3.23.40 AM.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Ensure that a pay run is open before performing this step.

WTT adjustments cannot be processed unless linked to an active pay run.
{% endhint %}

4. Review your selected employees and confirm that the adjustment amounts are correct.
5. Click “Accept” to proceed

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 3.35.16 AM.png" alt=""><figcaption></figcaption></figure>

6.  A confirmation pop-up will appear asking you to verify the changes.

    → Click “Confirm” to finalize.

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 3.35.35 AM.png" alt=""><figcaption></figcaption></figure>

7. Once successful, a confirmation message will appear indicating that the WTT adjustments have been applied.

<figure><img src="../../.gitbook/assets/Screenshot 2025-10-22 at 3.35.44 AM.png" alt=""><figcaption></figcaption></figure>

#### Final Tip

Review the WT Projection Tool regularly - especially before each payroll run near the end of the third quarter and in the months leading up to year-end - to keep your tax projections on track and help prevent over- or under-withholding.
