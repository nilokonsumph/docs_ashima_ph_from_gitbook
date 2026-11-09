# configure Post Payroll Adjustment availability

use **Post Payroll Adjustment Settings** to control whether eligible corrections from a previous closed payroll can enter the PPA process. an approved PPA is brought forward to the current open pay run so that an underpayment or overpayment can be handled on the next transaction date.

**navigation:** go to **Settings → Paycheck → Post Payroll Adjustment**.

## choose who can start a PPA

| setting                                       | effect                                                                                                                                              |
| --------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Enable Post Payroll Application (PPA)** off | blocks new use of the PPA process for the company                                                                                                   |
| **Enable Post Payroll Application (PPA)** on  | allows eligible PPA corrections within the saved prior-payroll limit                                                                                |
| **Employee Initiated PPA (Optional)** off     | administrators can initiate an eligible PPA on an employee's behalf; the admin-initiated request is treated as approved without a Workflow decision |
| **Employee Initiated PPA (Optional)** on      | employees can submit their own eligible PPA requests; those requests follow the applicable approval Workflow                                        |

PPA applies to the supported late time and attendance corrections shown by Ashima: timesheet adjustments, missed time logs, missed rest-day requests, leaves, and missed overtime. enabling the setting does not make every historical payroll item editable.

## set the eligible prior-payroll limit

use **PPA Limit** to choose from one to six previous payroll dates. the saved number limits how far back an otherwise eligible PPA request can reach. it does not reopen those payrolls or change their closed status.

## update the company setting

1. review pending PPA approvals before changing availability.
2. turn **Enable Post Payroll Application (PPA)** on or off.
3. when PPA is on, decide whether employees may initiate requests.
4. select the **PPA Limit** from one to six previous payroll dates.
5. save the page.

{% hint style="warning" %}
**warning:** Ashima blocks disabling PPA when a timesheet, leave, or overtime PPA request is still pending. approve or reject those requests first, then return to the setting.
{% endhint %}

\## verify the result

reopen **Post Payroll Adjustment Settings** and confirm the saved options, updater, and updated date. use an eligible controlled record to confirm that the expected initiation path is available. for an employee-initiated test, verify that the request reaches Todo; for an administrator-initiated test, verify the resulting PPA record and its carry-forward into the applicable open pay run.

if the expected path is unavailable, check the company setting, prior-payroll limit, source record type, employee or administrator access, Workflow, and payroll state before retrying. changing this setting does not rewrite a closed pay run or resolve a pending request.

## continue in the affected module

* [review Post Payroll Adjustments in Paycheck](../../paycheck/corrections-controls-and-ingestion/use-post-payroll-adjustments.md#post-payroll-adjustments-ppa)
* [review PPA approval work in Todo](../../todo-workflow/)
* [review late time corrections in Hours](../../hours/)
* [review late leave corrections](../../leaves-cto/)
