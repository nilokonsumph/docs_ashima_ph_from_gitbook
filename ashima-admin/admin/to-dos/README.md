# To Do's

***

use **Todo** to find requests waiting for your review. The **Workflow** setting determines which approver receives each request, whether another approval level follows, and whether the workflow applies company-wide or only to assigned employees.

**Navigation:**\
go to **Todo**.

### what types of requests appear in Todo?

the Todo page groups pending work by request type and shows a badge count when matching items are available. Request types may include:

* **time and attendance:** Timesheets, Rest Day, Holiday, Mobile Clock-in, Open Shifts, Overtime, and Shifts;
* **leave and benefits:** Leave and Maternity; and
* **payroll and company processes:** Payroll, Documents, Disbursement, 13th Month, Year End, and Termination.

the categories you see depend on your privileges, workflow assignment, enabled modules, and pending requests.

### how are Todo and Workflow connected?

Todo displays approval work; it does not decide who the approver is. That routing is managed under **Settings → Workflow**.

1. a user creates or submits a request in its source module.
2. the applicable workflow identifies the current approver or approval level.
3. the request appears in that approver's Todo queue.
4. approval either completes the request or moves it to the next approval level. Rejection returns or closes the request according to that module's rules.

an administrator should update the Workflow page—not the Todo queue—when the approver, approval order, or employee assignment must change.

### what workflow is available at the start?

Ashima starts supported processes with a default workflow that uses one approval level assigned to the Ashima owner account. An administrator can create a custom workflow with different managers, more than one approver at the same level, or multiple approval levels where the process supports them.

when multiple approvers are assigned to the same level, all approvers at that level must approve before the request progresses. In a multi-level workflow, level 1 must finish before level 2 receives the request.

### which workflows are company-wide?

the following processes use one current workflow across the company:

* Payroll;
* Disbursement;
* Documents;
* 13th Month;
* Year End; and
* Termination.

for these processes, creating a new workflow replaces the current company-wide workflow. Employees do not need to be reassigned individually. Before replacing it, finish or review requests still pending under the current workflow.

### which workflows can differ by employee or group?

supported employee-scoped workflows can be assigned to different employees or groups. For example, one group of employees may use one Leave approval workflow while another group uses a different Leave workflow and approvers.

Leave is centralized under its assigned workflow by default. If advanced leave-type routing is enabled for the company, each leave type can instead have its own workflow assignment, approvers, and approval levels. This option must be configured before administrators assign separate workflows by leave type.

### related articles

* approval queue
* workflow settings
