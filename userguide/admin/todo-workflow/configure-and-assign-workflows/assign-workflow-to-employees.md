# assign Workflow to employees

## assign Workflow to employees

employee-scoped processes can use different Workflows for different employees. use this when teams, locations, or operating groups need different approvers for the same type of request.

### distinguish company-wide and employee-scoped routing

company-wide processes use the one current route described in [choose the Workflow model for the process](configure-an-approval-workflow.md#choose-the-workflow-model-for-the-process). supported attendance, Leave, and other employee processes can have several Workflows assigned to different employees. standard Leave uses the assigned Leave Workflow; Leave-type-specific routing appears only when the company's advanced Leave Workflow option is enabled.

### assign or reassign an employee

1. create and verify the target Workflow.
2. open the employee's employment details and Workflow assignment area, or the employee-assignment area in Workflow details.
3. select the process and target Workflow.
4. review the current and target level counts and approvers.
5. save the assignment.
6. reopen the employee record and verify the active Workflow.

when an employee has a pending application, Ashima blocks reassignment to a Workflow with fewer approval levels than the current Workflow. complete the pending request or select a compatible Workflow with at least the current number of levels. moving to the same or a higher level count is not subject to that specific fewer-level guard, but still requires a review of current approvers and pending work.

{% hint style="warning" %}
**warning:** do not treat employee reassignment as a way to bypass a pending approver. confirm how the existing request is routed before changing the employee's future assignment.
{% endhint %}

\## verify employee coverage

download or review the Workflow assignment list when you need to confirm which employees use a Workflow. check unassigned employees, recent hires, transfers, and employees whose approval route changed. a Workflow definition without the intended employee assignment will not route an employee-scoped request as planned.

if the wrong Workflow was assigned, select the correct compatible Workflow and save again. when a pending-request guard blocks the correction, complete or resolve the pending request first; do not unassign the employee or reduce the approval path to bypass the guard.
