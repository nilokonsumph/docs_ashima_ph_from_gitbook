# handle locked and changed approval work

## handle locked and changed approval work

a Todo can remain pending even when its approval controls are temporarily locked or permanently unavailable. first identify whether the restriction comes from **Payroll Lock**, the pay run's processing status, the Workflow level, or an action already completed by another approver.

### what happens to administrator Todos when Payroll Lock is enabled?

**Payroll Lock** applies company-wide to payroll-sensitive work. it always prevents managers from approving or rejecting payroll-sensitive Todos. the additional **Lock payroll-sensitive Admin To-Dos** setting decides what happens in the administrator portal.

| Payroll Lock configuration                                                                | manager Todo decisions                                | administrator Todo decisions                                                         |
| ----------------------------------------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------ |
| **Enable Payroll Lock** is off                                                            | available when every other approval rule is satisfied | available when every other approval rule is satisfied                                |
| **Enable Payroll Lock** is on and **Lock payroll-sensitive Admin To-Dos** is selected     | suspended                                             | suspended                                                                            |
| **Enable Payroll Lock** is on and **Lock payroll-sensitive Admin To-Dos** is not selected | suspended                                             | authorized administrators can continue permitted Admin Todo approvals and rejections |

enabling the lock does not approve, reject, or delete an existing Todo. the affected request remains pending, but the decision control is locked. after Payroll Lock is disabled, the action becomes available again only when the payroll is still in a supported state, it is the signed-in administrator's turn, and no other restriction applies.

{% hint style="info" %}
**note:** Payroll Lock governs payroll-sensitive Todo decisions. it does not mean that every administrator action is disabled. the current configuration specifically keeps permitted administrator Leave and Overtime submissions available.
{% endhint %}

### what happens when the related pay run is waiting for approval?

affected time and attendance Todos for dates included in a pay run with **Waiting for approval** status are shown as **Locked for payroll processing**. they remain in the queue, but cannot be approved or rejected while the pay run is in that processing state. complete the payroll decision first. if the pay run returns to a supported editable state, reload the Todo queue and review the request again before acting.

### what happens when payroll closes before a pending Todo is decided?

pending **Timesheets**, **Leave**, and **Overtime** requests tied to the closed payroll can remain visible in Todo. Ashima marks them **Part of a Closed Payroll and cannot be Approved**. closing payroll does not silently approve or remove them.

where the queue identifies closed-payroll items, it provides a count and a control to reject all of those closed-payroll applications. open the identified list and review the affected employees, dates, and requests before confirming the bulk rejection. the rejection removes the obsolete pending work from the queue; it does not reopen or recalculate the closed payroll.

{% hint style="warning" %}
**warning:** do not use the closed-payroll cleanup as a substitute for a payroll correction. if the closed payroll is wrong, follow the supported post-payroll correction or adjustment process. a request explicitly returned through a supported resend or post-payroll correction flow can have a different action state; follow the controls and warning shown on that returned record.
{% endhint %}

### what happens if an approver resigns or becomes inactive?

changing an approver's employment status to **Inactive** or **End of Employment** does not automatically move that person's Workflow levels to the default Workflow or its approver. the saved Workflow and level still exist, but an inactive or former approver should no longer be relied on to receive or decide the work. **End of Employment** also removes the person's login identifiers, so that account cannot be expected to complete pending approvals.

when the employment-status change is saved, Ashima checks whether the person's account owns any Workflow levels. if it does, the employee-status flow lists the affected Workflows and asks the administrator to select a replacement approver for each one. company-wide Payroll, Document, Disbursement, 13th Month, End of Year, and Termination Workflows require an eligible owner or administrator replacement. other supported employee-scoped processes can show the eligible replacement choices allowed by that Workflow.

1. review every affected Workflow and approval level shown during the status change.
2. select an active replacement approver for each listed level.
3. submit the reassignment.
4. open **Settings → Workflow** and verify that the former approver no longer owns an active level.
5. review pending Todos for each affected process and confirm that the replacement can see and act on the current-level requests.

if another active approver is already assigned at the same level, that remaining approver can still complete the level. reassign the former approver anyway so future requests do not depend on an inactive account.

{% hint style="warning" %}
**important:** the default Workflow is not automatic absence or resignation cover. add more than one approver at a level when operational cover is needed, and reassign Workflow ownership as part of the administrator's offboarding checklist.
{% endhint %}

if the status was already changed without completing reassignment, update the affected Workflow levels immediately. pending requests do not become default-Workflow requests merely because their assigned approver became inactive.

### other common what-if situations

| situation                                                                         | what happens                                                                                                                                              | what the administrator should do                                                       |
| --------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| the request is visible through view-all access, but it is not your approval level | the row can be visible while its decision control is locked                                                                                               | review the approver trail and leave the decision to an approver at the current level   |
| another approver at your level acts first                                         | that approval level is completed once; the request advances or reaches final approval                                                                     | reload the queue and verify the saved action instead of trying to decide the stale row |
| the request has more approval levels                                              | completing the current level advances it to the next configured level                                                                                     | do not treat the first approval as final unless it is the last level                   |
| a request is rejected                                                             | the rejected outcome is saved; Ashima does not create a corrected replacement automatically                                                               | correct the source record and submit again through the source module when needed       |
| an approver becomes inactive or reaches End of Employment                         | the default Workflow does not automatically replace that approver; the affected level can depend on the remaining same-level approvers or become stranded | assign an active replacement to every affected Workflow level and verify pending Todos |
| Payroll Lock is removed but the row is still locked                               | another rule still applies, such as **Waiting for approval**, **Closed**, current-level ownership, privilege, or company scope                            | read the row warning and approver trail, then resolve that specific condition          |
| a bulk action contains the wrong records                                          | confirmation applies the decision to the selected rows                                                                                                    | cancel, correct the selection and selected-item count, then confirm again              |
