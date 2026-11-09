# understand locked, closed, and reassigned approval work

the state of the related process can change what you can do with a request:

* when a pay run is frozen, the freeze option determines whether administrators and approvers can continue applicable To Do work; read the current freeze notice rather than assuming every lock behaves the same way;
* when the related payroll is closed, unresolved requests do not automatically rewrite that closed payroll;
* when a request is already approved, rejected, cancelled, or acted on by another approver, refresh the queue before trying another action;
* when an approver becomes inactive or leaves employment, existing workflow setup must be reviewed and reassigned by an administrator; do not assume that every pending request automatically falls back to the root owner;
* a default workflow provides a fallback configuration for its workflow family, but it is not proof that an inactive approver's pending item has been reassigned.

ask the workflow or payroll administrator to review the exact request, workflow level, approver status, and payroll state when a pending item cannot be acted on. see [handle locked and changed approval work](../../../admin/todo-workflow/review-approval-work/handle-locked-and-changed-approval-work.md).

## what should i do in each state?

| state                                    | manager action                                                                                         |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| payroll frozen but approver work allowed | complete only the actions still enabled by the freeze option                                           |
| payroll frozen and approvals suspended   | stop and wait for payroll administration to change the lock                                            |
| payroll closed                           | do not approve an old request expecting it to rewrite pay; use the eligible PPA process when available |
| request already acted on                 | refresh the queue and use the resulting status                                                         |
| approver inactive or no longer employed  | ask the workflow administrator to replace the approver and review pending assignments                  |
| employee or request moved out of scope   | ask the administrator to confirm current manager scope and workflow ownership                          |

include the company, employee, request type, source date or pay period, workflow level, former approver, and displayed message when escalating.
