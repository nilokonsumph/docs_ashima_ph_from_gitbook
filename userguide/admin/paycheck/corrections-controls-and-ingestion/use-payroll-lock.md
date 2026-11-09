# use Payroll Lock

## use Payroll Lock

### how do I use freeze pay run?

use Payroll Lock while finalizing payroll to pause covered employee and manager changes. choose separately whether to pause payroll-sensitive Admin To-Do decisions. the setting applies company-wide; it is not limited to the run you are viewing, and individual administrators cannot be selected.

from the Pay Run workspace, click the freeze icon to open **Payroll Lock settings**. this modal can be configured directly. the separate **payroll lock** page remains another entry point and has its own edit controls.

#### which lock options should I choose?

| configuration                                                 | employee and manager effect                                                                                                                                  | administrator effect                                             |
| ------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------- |
| **Enable Payroll Lock** off                                   | this freeze does not suspend covered activity                                                                                                                | this freeze does not suspend Admin To-Do decisions               |
| main lock on; **Lock payroll-sensitive Admin To-Dos** checked | employees cannot submit covered payroll-sensitive applications; managers retain view access but cannot make covered changes or approve/reject covered To Dos | admins cannot approve or reject covered payroll-sensitive To Dos |
| main lock on; additional admin restriction unchecked          | employee and manager restrictions remain                                                                                                                     | authorized admins can continue permitted Admin To-Do decisions   |

the additional admin restriction appears when the main lock is enabled and is selected by default. other permitted admin actions remain available, including admin leave and overtime submissions. this is not a freeze of every admin function.

#### how do I apply the selection?

1. open **Payroll Lock settings** using the freeze icon.
2. set **Enable Payroll Lock**.
3. when enabling it, keep **Lock payroll-sensitive Admin To-Dos** checked to pause those decisions, or uncheck it to allow authorized admins to continue them.
4. read **Configured behavior**. it changes with your selections and summarizes who will be restricted.
5. click **update**. the password confirmation describes enabling/disabling the lock and warns when admin To-Do approvals will also be frozen.
6. complete password confirmation and select **yes, update** to submit the change.
7. check the saved lock state before continuing payroll preparation.

use **cancel** to leave the settings modal without submitting the selections. changing a checkbox or reaching password confirmation does not itself save the lock.

#### what should I watch out for?

turning the main lock off hides the additional restriction. the admin restriction returns to its default checked state for the next freeze, so review it each time you enable the lock.

when admins remain permitted to make payroll-affecting changes, those changes can still require recalculation before payroll submission. freezing inputs does not itself recalculate payroll or prove that the current amounts are ready.

the company freeze and restrictions attached to waiting/closed payroll are different controls. turning this freeze off does not make a closed payroll editable.

***

### payroll lock

#### what should administrators know about locked requests?

once payroll is already **Waiting for approval** or **Closed**, the original pay run should be treated as no longer changeable through normal payroll review.

some payroll-affecting requests may still appear in review or **To Do**, but they can show **Locked for payroll processing** or behave as no longer approvable through the original payroll cycle.

#### what happens to requests that come in after payroll is already in approval or closed?

once a pay run is **Waiting for Approval** or **Closed**, it should be treated as no longer changeable through normal payroll review. This applies to:

* admin-initiated payroll-affecting updates
* late employee timesheet, overtime, or leave requests
* late manager approvals for payroll-affecting items

requests submitted after the payroll moved forward can become locked. the portal may show these items with a lock indicator and the note **Locked for Payroll Processing**.

if the payroll is already closed, the request can show that it is connected to a closed payroll and can no longer be approved through the original pay run.

do not approve these requests through the original pay run. See [Post Payroll Adjustments ](../start-here-understand-paycheck.md#page-070-pages-admin-paycheck-md--what-are-post-payroll-adjustments-ppa)below for the correct process.

{% hint style="info" %}
a timesheet locked while payroll is waiting for approval cannot proceed through the normal edit flow. PPA applies to eligible closed-payroll corrections; do not reinitiate a request solely because the payroll is waiting for approval.
{% endhint %}

#### what should I do with expired Todo items?

some payroll-affecting requests remain visible in **To Do** even after the connected payroll is no longer available for normal approval.

when this happens:

* the item may remain listed for visibility and follow-up but is no longer actionable as a normal open-pay-run approval.
* if the request still shows a pending action, the approver should reject it so it is cleared from the original approval flow.
* if the correction still needs to be processed, re-initiate it through Post Payroll Adjustments instead of approving from the old To Do item.

***
