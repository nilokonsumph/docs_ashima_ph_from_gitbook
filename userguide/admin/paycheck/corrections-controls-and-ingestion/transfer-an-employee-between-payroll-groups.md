# transfer an employee between payroll groups

## transfer an employee between payroll groups

use **Transfer Paygroup** to move an eligible employee between non-confidential and confidential payroll handling through the controlled transfer workflow.

**Navigation:**\
open **Transfer Paygroup** from the payroll-group/confidential-employee workflow available to your role.

{% hint style="warning" %}
starting a transfer moves the employee into a temporary transfer payroll group. Complete or revert the pending transfer; do not leave the employee in the temporary state without an owner and next action.
{% endhint %}

### how do I start a transfer?

1. open **Transfer Paygroup**.
2. select **assign to**.
3. choose **Transfer to Confidential** or **Transfer to Non-Confidential** when both directions are permitted.
4. search for and select the employee.
5. select the matching transfer action.

only active employees on the correct source-confidentiality side and not already in transfer are eligible. An employee with a blocking draft pay run cannot be transferred unless the employee is validly excluded from that blocking draft under the current rule.

### how do I finalize a pending transfer?

open the matching received-transfer page, select the employee, choose an eligible receiving payroll group, and select **finalize selected**. The receiving group must:

* match the destination confidentiality;
* have no blocking draft pay run; and
* remain within the 150-employee capacity after all selected transfers.

the page also supports search and download of pending transfers.

### how do I revert a pending transfer?

use the row action on the received-transfer page, select a valid payroll group on the original confidentiality side, and confirm the revert. Revert clears the transfer state but requires an explicit destination group; do not assume the system silently restores the former group.

### audit and payroll effect

start, finalization, and revert write transfer history/audit details. Finalization changes the employee's confidentiality and payroll group. Review employee access, payroll-group membership, and the next payroll after completion.

### related articles

* [create or delete a draft pay run](../run-payroll/create-or-delete-a-draft-pay-run.md#page-073-pages-admin-paycheck-run-payroll-create-or-delete-a-draft-pay-run-md)
* [payroll exclusions](../run-payroll/exclude-or-include-an-employee.md#page-077-pages-admin-paycheck-run-payroll-payroll-exclusions-md)
* [payroll masterlist and readiness](../run-payroll/review-the-payroll-masterlist-and-readiness.md#page-076-pages-admin-paycheck-run-payroll-payroll-masterlist-and-readiness-md)
