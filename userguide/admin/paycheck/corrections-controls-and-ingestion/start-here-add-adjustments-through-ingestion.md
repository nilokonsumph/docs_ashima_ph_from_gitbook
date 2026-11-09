# start here: add adjustments through ingestion

use Ingestion to add supported employee pay items to an existing source record such as an open paycheck, termination, end-of-year process, 13th Month run, or disbursement. the page receives its source type and source ID from the owning workflow; it is not a separate payroll run.

## understand the source boundary

| source type  | how ingestion is used                                                                                                         |
| ------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| paycheck     | add supported items to the selected open pay run; calculation categories can be limited unless the calculator view is enabled |
| termination  | add supported items for the selected employee and termination record                                                          |
| end of year  | add supported year-end amounts using the categories allowed for that source                                                   |
| 13th Month   | add supported 13th Month items or adjustments to the selected run                                                             |
| disbursement | add supported items to the selected disbursement source                                                                       |

{% hint style="warning" %}
**warning:** confirm the employee, source type, source record, period, pay date, category, item, tax status, and amount before saving. ingestion changes an input to the owning calculation; it does not prove that the result was approved, closed, paid, or filed.
{% endhint %}

\## continue in the owning modules

* [review and recalculate Paycheck](../)
* [configure earning, deduction, loan, and contribution items](../../settings/)
* [review employee assignments](../../workforce/)
* [review Disbursement](../disbursement/)
