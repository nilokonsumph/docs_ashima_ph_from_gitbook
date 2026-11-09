# review premium-work requests

## review premium-work requests

use **Overtime** or the applicable **Timesheets** Rest Day or Holiday view to confirm that recorded work is eligible before it is paid or converted to CTO.

review the employee, work date, assigned shift, rest-day or holiday classification, clock-in and clock-out, eligible minutes or hours, prior approval, payroll use, and CTO status. confirm that the same source work has not already been paid or converted.

### choose payroll approval or CTO

where CTO is enabled and the selected Rest Day or Holiday items are eligible, the queue can offer **Approve as CTO**. approve payroll items and CTO items separately. Ashima blocks a mixed decision when selected records do not all support the chosen action or when an item is already pending CTO minting.

approval for payroll makes the accepted source available to the applicable payroll process. **Approve as CTO** sends eligible source work to the CTO conversion flow. rejection keeps the captured time but does not make the rejected premium application payable.

{% hint style="warning" %}
**warning:** choosing **Approve as CTO** changes the intended result from pay to compensatory time. review the employee, eligible minutes, CTO rules, expiry behavior, and existing use before confirming.
{% endhint %}

### why can Rest Day work appear without an employee application?

when Rest Day approval is enabled, an approved employee application normally authorizes inclusion of the work in payroll review. an administrator can also enable inclusion when adding or updating the record.

if you do not see an employee application, review the log source and history before treating the record as incorrect. confirm the assigned schedule, day type, employee entitlement, and actual hours, then recalculate the affected open payroll and review the result.

{% hint style="info" %}
including Rest Day work does not by itself guarantee premium pay. the schedule, entitlement, day type, hours, and payroll calculation still determine the amount.
{% endhint %}
