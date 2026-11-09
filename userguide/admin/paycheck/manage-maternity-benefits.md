# manage maternity benefits

## manage maternity benefits

***

### maternity benefits

Use **Maternity Benefits** to follow a maternity application from filing and approval through the SSS-based calculation, company salary differential, disbursement, reimbursement tracking, and any return to work during the leave period.

**Navigation:** go to **Leaves → Maternity Benefits** to review employee records. Use **To Do's → Maternity Benefits** for applications waiting for an approval decision. Previous-employer contribution records are maintained through **Settings → Imports → Previous SSS Contribution** when that page and privilege are available.

The employee's maternity application and the administrator's calculated maternity record are related parts of one workflow. Filing or approving the application does not by itself confirm that the contribution history, calculated amount, reimbursement, and affected payroll have all been reviewed.

#### before you begin

Confirm:

* the employee, expected date of delivery or contingency date, leave start date, and maternity leave type;
* whether the employee selected the standard 105-day leave, the 120-day solo-parent option, or the 60-day emergency-termination option shown by the application;
* whether up to seven days are allocated to an alternate caregiver and, when applicable, the selected employee;
* that the employee's SSS contribution history is complete for the displayed 12-month contribution period;
* whether missing months belong to payroll processed in Ashima or to a previous employer;
* the employee's current basic pay and the company choices for employee SSS, PhilHealth, and HDMF contributions during maternity leave;
* the required approval route and current application status; and
* any open payroll that overlaps the maternity period or an early-return date.

{% hint style="warning" %}
An incomplete contribution history can prevent the calculation or understate the monthly salary credits used. Do not substitute the employee's current salary for missing contribution months.
{% endhint %}

#### how does an employee apply for maternity benefits?

From the employee maternity-benefit application, the employee:

1. chooses the **Maternity Leave Type**;
2. indicates whether leave credits will be allocated to an alternate caregiver;
3. enters the allocation, from one to seven days, and selects the alternate caregiver when applicable;
4. reviews the resulting **Length of Leave**;
5. enters the **Leave Start Date** and expected childbirth date;
6. enters the reason or supporting application information shown by the form; and
7. submits the application for the configured approval workflow.

The dates and selected leave type determine the leave period and feed the maternity calculation. If an administrator files or corrects a record on the employee's behalf, use the same employee-approved dates and supporting information.

#### what happens during approval?

Pending maternity applications appear in the maternity approval queue for the assigned approver. An authorized approver can open the employee detail, review the application, select one or more eligible records, and approve or reject them. The queue also supports a list download when the action is available.

Approval advances the maternity application. Rejection returns it from the approval path for correction or follow-up. The current approval actions do not capture an approver note, so confirm the employee, dates, leave type, alternate-caregiver allocation, and supporting records before deciding.

{% hint style="warning" %}
Approval confirms the application decision. It does not replace the administrator's review of the contribution source, calculation detail, reimbursement record, early return, or payroll result.
{% endhint %}

#### what can I do from the maternity benefits list?

Depending on access and record state, the list allows you to:

* search or filter maternity-benefit records;
* open an employee's maternity details;
* review the leave period, maternity and application statuses, and key amounts;
* update the supported filed, reimbursement, and advance or early-return sections;
* print the employee's maternity output; and
* download the available list.

Confidential employees and actions remain subject to the user's access. A record shown on the list is not necessarily approved, reimbursed, or complete.

#### where do the contribution months come from?

Ashima first reads the employee's active Ashima payroll payslips whose payroll dates fall within the displayed 12-month contribution period. When an employee has more than one payroll in a month, the system combines the applicable SSS contribution values for that month before deriving its monthly salary credit.

For a new employee or an employee whose required months were processed outside the current Ashima company record, maintain **Previous SSS Contribution** records. The import flow provides a template, validates the uploaded file, allows a retry when validation fails, and saves the accepted contribution records. These records supplement the history used by the maternity calculation; they do not create Ashima payslips for the prior employer.

After an import or correction, reopen the maternity record and confirm that the expected months, contribution values, and monthly salary credits appear. If Ashima reports missing SSS remittance records, complete or correct the contribution history before relying on the benefit result.

#### how does Ashima select the calculation period?

The calculation detail shows the sequence used for the employee record:

1. **Expected Date of Delivery** identifies the contingency date.
2. **Quarter of Contingency** shows the calendar quarter containing that date.
3. **Semester of Contingency** identifies the related six-month semester.
4. **12 Month Contribution Period** covers the 12 months immediately before the semester of contingency.
5. Ashima converts each supported month's SSS contribution to a **Monthly Salary Credit** using the applicable table available to the calculation.
6. The calculation uses up to six selected monthly salary credits from the displayed contribution period for the benefit basis.

Review the actual date range and every displayed month. Changing the expected delivery date can change the quarter, semester, 12-month source window, and calculated benefit.

#### how is the SSS maternity benefit calculated?

The calculation page labels the main values as follows:

| value                       | calculation or meaning                                                                      |
| --------------------------- | ------------------------------------------------------------------------------------------- |
| total monthly salary credit | sum of the selected monthly salary credits, using up to six months                          |
| daily maternity allowance   | total monthly salary credit ÷ 180 days                                                      |
| approved maternity days     | the approved length from the maternity leave type and allocation                            |
| SSS maternity benefit       | daily maternity allowance × approved maternity days, subject to the limit applied by Ashima |

**Calculation relationship**

`SSS maternity benefit = (sum of selected monthly salary credits ÷ 180) × approved maternity days`

**Worked arithmetic example**

If the six selected monthly salary credits total **PHP 120,000** and the employee has **105 approved days**:

1. daily maternity allowance = PHP 120,000 ÷ 180 = **PHP 666.67**;
2. benefit before the system limit = PHP 666.67 × 105 = **PHP 70,000.35** using the rounded daily value; and
3. Ashima applies its supported rounding and benefit limit to produce the displayed SSS maternity benefit.

Use the displayed system result as the payroll record. The example explains the arithmetic and is not a substitute for confirming the employee's source months and the statutory table used by the company.

#### how are full pay, salary differential, and total disbursement related?

Ashima displays these additional values:

| value                          | calculation or meaning                                                                                              |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------------- |
| basic pay                      | employee basic pay used for the maternity record                                                                    |
| maternity period in months     | approved maternity days converted using 30 days per month for the full-pay calculation                              |
| full pay                       | basic pay × approved maternity days ÷ 30; Ashima does not leave full pay below the calculated SSS maternity benefit |
| employee premium contributions | employee SSS, PhilHealth, and HDMF shares included according to the maternity contribution choices                  |
| salary differential            | full pay − SSS maternity benefit − employee premium contributions, with a minimum of zero                           |
| total disbursement             | full pay − employee premium contributions                                                                           |

These values answer different questions. The SSS maternity benefit comes from the contribution history. Full pay uses the employee's basic pay and approved maternity period. Salary differential is the remaining company amount after the SSS benefit and supported employee premium contributions. Total disbursement is the resulting amount shown for disbursement.

{% hint style="warning" %}
Do not add the displayed salary differential to total disbursement. Total disbursement already represents the full-pay result after supported employee premium contributions.
{% endhint %}

#### what should I review in employee details?

Review:

* maternity leave type, approved length, leave start and end dates, and expected date of delivery;
* alternate-caregiver allocation when applicable;
* date filed, record status, application status, and approver progress;
* quarter and semester of contingency and the complete 12-month contribution period;
* contribution and monthly salary credit for each displayed month;
* the selected monthly salary credits and their total;
* daily maternity allowance, approved days, and SSS maternity benefit;
* basic pay, full pay, employee premium contributions, salary differential, and total disbursement;
* SSS notification, transaction, approved-day, reimbursement, and update information;
* working-during-leave or early-return settings; and
* the last person and date that updated the supported sections.

Do not infer an employee value from another record. Dates, contributions, salary, leave type, allocation, company settings, and workflow state can all change the result.

#### how do I update a maternity record?

1. Find and open the employee's maternity-benefit record.
2. Review the application, approval status, and maternity dates.
3. Reconcile the 12-month contribution table with Ashima payroll payslips and Previous SSS Contribution records.
4. Review the calculated benefit, full pay, premium contributions, salary differential, and total disbursement.
5. Update only the filed, reimbursement, advance, or early-return fields supported by the page and your role.
6. Save the applicable section.
7. Reopen or refresh the record and verify the saved values and calculated result.
8. Review any affected open payroll and recalculate it when required.

#### how do I maintain SSS reimbursement information?

use the reimbursement section to record the transaction number, notification filing date, approved maternity days and reimbursed amount. an **Approved** record and edit permission are required. follow [save and verify SSS reimbursement information](../leaves-cto/maternity-and-sss-records/calculate-and-maintain-maternity-benefits.md#how-do-i-maintain-sss-reimbursement-information) for the section's **Edit**, **Save**, password confirmation, error correction and **Cancel** steps.

reimbursement tracking records what SSS has processed. it does not recalculate the source contribution months or replace payroll review. reopen the record to verify the saved reimbursement values rather than using the calculation's update time as proof of this save.

#### how does an early return affect payroll?

Use the advance or early-return section only when the employee will work during maternity leave or has an approved effective return date. Compare the return date with the displayed maternity end date and each overlapping payroll period.

After saving, review and recalculate the affected open payroll. The original maternity result and ordinary pay should not be assumed to remain correct when the employee returns during the approved leave period.

{% hint style="warning" %}
A maternity date, contribution-history, contribution-choice, or early-return change can alter the calculated amount or payroll result. A successful save is not the end of the review.
{% endhint %}

#### what outputs are available?

Depending on record state and access, Maternity Benefits provides the employee detail, maternity print or payslip output, and list download. The approval queue can also provide its supported list download.

Before treating an output as final, confirm that its employee, leave period, source months, calculation totals, approval state, and reimbursement or early-return information agree with the detail page.

#### what should I check before approval or output?

* employee, leave type, allocation, and dates;
* application and approval status;
* complete 12-month contribution history, including previous-employer records when applicable;
* selected monthly salary credits and calculated SSS maternity benefit;
* full pay, employee premium contributions, salary differential, and total disbursement;
* reimbursement and supported early-return information;
* effect on every overlapping open payroll;
* completed recalculation when required; and
* consistency between the detail page and the available print or download output.

#### related articles

* configure Paycheck before running payroll
* review leave and maternity requests
* import Previous SSS Contribution records
* review and recalculate a pay run
* review employee pay details
* definition of terms
