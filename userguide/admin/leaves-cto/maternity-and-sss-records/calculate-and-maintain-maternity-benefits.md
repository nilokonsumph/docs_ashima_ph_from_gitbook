# calculate and maintain maternity benefits

## calculate and maintain maternity benefits

use maternity benefits to review the calculation values shown for an employee record. maternity benefits is a separate workflow from ordinary leave balances and compensatory time off.

**Navigation:**\
go to **Paycheck → Maternity Benefits**.

### before you begin

confirm:

* the correct employee and maternity record;
* the applicable maternity dates and supporting information;
* employee eligibility and current status;
* company maternity and approval settings;
* SSS-related information available for the employee; and
* any open payroll affected by the benefit.

### how do i find the maternity record i need?

depending on access and record state, the list allows you to:

* search or filter maternity-benefit records;
* open an employee's maternity details;
* review current status and key dates; and
* download the available list or report.

select an ordinary employee row to review its detail. when shown, **view details / edit** opens the update view directly; it is a different route from the row detail. the list download is separate from the employee-detail export.

### what should i review in employee details?

review:

* maternity leave type and allocated credits;
* alternative caregiver information when applicable;
* leave length, start date, end date, and expected date of birth;
* date filed, record status, application status, and approver progress;
* the SSS contribution period used by the calculation;
* total monthly salary credit and daily maternity allowance;
* approved maternity days and computed SSS maternity benefit;
* full pay, employee contributions, salary differential, and total disbursement;
* SSS notification, transaction, approval, and reimbursement information;
* working-during-leave or early-return settings; and
* the last person and date that updated the supported sections.

use the displayed fields and current company setup. do not infer an employee value from another employee's record because eligibility, dates, compensation, reimbursement, and payroll status can differ.

from the employee detail, open the relevant record row to reach its update view. use the detail page's **XLS** or **CSV** export for that employee's records.

### how do i update a maternity record?

1. find the employee and open the record's update view.
2. review the application, dates, calculation, and approval state.
3. select **Edit** for the record section when available. change only the fields supported by your access and record state.
4. select **Update** to keep those record changes, or **Cancel** to leave them. **Submit for Approval** is a separate action when the record is ready and the button is available.
5. use the SSS reimbursement and early-return sections' own controls for those changes, as described below.
6. review the saved result and any affected open payroll; recalculate that pay run when required.

### how should i read the calculation section?

the maternity detail page explains the calculation in stages:

1. the contribution table identifies the monthly salary credits used and the displayed total monthly salary credit;
2. total monthly salary credit is divided by 180 days to obtain the displayed daily maternity allowance; and
3. the daily allowance is multiplied by the approved maternity days to obtain the displayed SSS maternity benefit.

review the displayed months and values for the employee record rather than copying another employee's result.

### how do i maintain SSS reimbursement information?

use this section to record reimbursement progress after the maternity record is **Approved**. you also need edit permission. reimbursement information does not replace the benefit calculation or payroll review.

1. choose **Edit** in **SSS Maternity Notification/Reimbursement Details**.
2. enter **Transaction Number**, **Notification Filing Date**, **Approved Maternity Days**, and **Reimbursed Amount** from the reimbursement evidence.
3. choose **Save** and complete the password confirmation. this saves only the reimbursement section.
4. if a field error appears, correct that field and save again. after success, check the four reimbursement values displayed.
5. reopen or reload the record and confirm the saved values. check this section's **Updated Date** when populated; an initial entry may have no updated date.

choose **Cancel** while editing to restore the saved reimbursement values. **Updated By**, when displayed, identifies the reimbursement updater. the calculation's **Updated Last** is a separate display time; use the saved reimbursement values to confirm this change.

### how does early return to work affect the record?

use the advance or early-return section only when the employee will work during maternity leave or has an approved effective return date. review the displayed maternity end date and payroll periods before saving.

an early-return record changes the period that needs payroll review. confirm the effective date and recalculate affected open payroll rather than assuming the original maternity result remains unchanged.

when available, this section uses **Edit → Update/Cancel**. review the revised date and its effect on the open payroll after updating.

{% hint style="warning" %}
**warning:** a maternity-benefit change can alter payroll. do not treat a saved record as fully reviewed until the affected payroll result has been checked.
{% endhint %}

\## how do settings affect the result?

company maternity settings define the available product behavior. employee eligibility, dates, compensation, recorded benefit information, and workflow state determine the employee result.

when the visible options differ from another company or employee, review the company setting and employee record before treating the difference as an error.

### what happens after saving?

Ashima stores the updated maternity-benefit information. the changed record can affect the employee's related payroll and available maternity output. review any open payroll and approval queue that uses the record.

### which maternity output should i retain?

depending on the record and access, maternity benefits provides employee detail, print or maternity payslip output, and list download. use the approved or completed record state required by the company process before treating the output as final.

to print a maternity payslip, select **Print** from the record's update view. review the print page, then select its **Print** action. this is separate from the list and employee-detail **XLS** or **CSV** exports.

### what should i check before approval or output?

* employee and dates;
* benefit and reimbursement information;
* supported early-return details;
* payroll effect;
* completed recalculation when required;
* status and approval state; and
* consistency between details and the available print or download output.

### related articles

* maternity settings
* [leave, CTO, and maternity benefits](../balances-transfers-and-cto/choose-between-leave-cto-and-maternity.md#page-065-pages-admin-leaves-leave-cto-and-maternity-benefits-md)
* [review and recalculate a pay run](../../paycheck/run-payroll/review-and-recalculate-a-pay-run.md#page-074-pages-admin-paycheck-run-payroll-review-and-recalculate-a-pay-run-md)
* [employee pay details](../../paycheck/run-payroll/review-employee-pay-details.md#page-075-pages-admin-paycheck-run-payroll-employee-pay-details-md)
* maternity approval queue

### verify the contribution months and formula

Ashima uses the employee's recorded contribution history and uploaded prior SSS contribution data where required. the calculation page identifies the contingency quarter and semester, reviews the twelve months before that semester, selects the six highest monthly salary credits, and displays the derived daily allowance and benefit components. the SSS formula is:

> \[!FORMULA] **average daily salary credit = total of the six highest applicable monthly salary credits ÷ 180**
>
> **SSS maternity benefit = average daily salary credit × compensable days**

the current SSS guidance uses 105 days for live childbirth, 120 days for a qualified solo parent, and 60 days for miscarriage or emergency termination of pregnancy. product results still depend on the employee record, saved contributions, company settings, approved dates, allocated credits, early return, and workflow state. review the twelve-month table and selected six months instead of entering only a final amount.

use **Previous SSS Contribution** when Ashima does not already hold the required prior contribution months, such as for a newer employee. the reimbursement section records transaction number, notification filing date, approved days, reimbursed amount, and update details; it does not replace the benefit calculation. password-gated changes must be reviewed after saving, and affected open payroll must be recalculated.

authoritative references: [SSS maternity benefit](https://www.sss.gov.ph/maternity-benefit/), [republic act no. 11210](https://lawphil.net/statutes/repacts/ra2019/ra_11210_2019.html), and its [implementing rules and regulations](https://lawphil.net/statutes/repacts/ra2019/irr_11210_2019.html).
