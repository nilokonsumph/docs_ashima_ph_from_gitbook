# configure approval Workflows

use Workflow settings to decide who reviews submitted requests, whether more than one approval is required, and whether the approval route applies company-wide or only to assigned employees.

{% hint style="warning" %}
**important:** changing an active workflow can affect approval routing. Review pending requests and the affected employees before replacing or reassigning a workflow.
{% endhint %}

\*\*navigation:\*\* go to \*\*Settings → Workflow\*\*.

## how are Workflow and Todo connected?

Workflow controls the approval route. Todo displays the requests currently waiting for the logged-in approver.

1. a request is submitted from its source module.
2. the applicable workflow identifies the current approver or approval level.
3. the request appears in that approver's Todo queue.
4. approval either completes the request or advances it to the next level.

changing the Workflow setting changes the routing setup; it does not approve the request from the Todo queue.

## what workflow is available at the start?

Ashima starts supported processes with a default workflow containing one approval level assigned to the Ashima owner account. Administrators can create custom workflows with different managers, multiple approvers at the same level, or multiple approval levels where the process supports them.

when multiple approvers are assigned to one level, any authorized approver at the current level can complete that level; Ashima does not wait for every same-level approver. In a multi-level workflow, the first level must finish before the next level receives the request.

## which workflows are company-wide?

the following processes use one current workflow for the company:

* Payroll;
* Disbursement;
* Documents;
* 13th Month;
* Year End; and
* Termination.

creating a new workflow for one of these processes replaces the current company-wide workflow. Employees do not need to be reassigned individually. Complete or review pending requests before replacing it.

## which workflows can be assigned to employees or groups?

supported employee-scoped workflows can differ by employee or group. For example, one employee group may use one Leave approval workflow while another group uses different approvers.

Leave uses its assigned workflow as a centralized route by default. If advanced leave-type routing is enabled for the company, each leave type can instead use its own workflow, approvers, and approval levels.

## how do i configure a workflow?

1. open the applicable request type under **Settings → Workflow**.
2. identify whether the workflow is company-wide or employee-scoped.
3. create or update the approvers and approval levels.
4. assign the workflow to the applicable employees or groups when assignment is supported.
5. review requests still pending under the current workflow.
6. save and confirm the intended approvers.

workflow assignment and page access are separate. An approver must also have the required module privileges and employee visibility.

## recover from incorrect routing

after saving, submit a controlled request and verify its current approver and level in Todo. if routing is wrong, review the process scope, employee or Leave-type assignment, active approvers, and pending requests before correcting the Workflow. do not delete or shorten a route to bypass a pending decision.

## continue in the affected module

* [manage requests in Todo](../../todo-workflow/)
