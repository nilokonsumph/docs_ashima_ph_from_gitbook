# create leave conversion and forfeiture reports

## create leave conversion and forfeiture reports

use **Reports → Leaves** to create a saved report for eligible unused leave that is converted to cash or forfeited under the configured leave policy. these reports help administrators review and retain the result for a selected leave type, employee scope, and period.

creating, deleting, or regenerating a report does not change the leave policy or correct an employee balance. review the applicable leave setting, employee balance, pending requests, and transaction ledger before creating the report.

### which report should i use?

| report               | use it to review                                  | check first                                                                                                       |
| -------------------- | ------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| **Leave Conversion** | eligible unused leave converted to a cash result  | monetization eligibility, conversion limit and schedule, pending requests, expired credits, and employee balances |
| **Forfeiture**       | eligible unused leave lost under the saved policy | unused-credit rule, carryover and expiry conditions, pending requests, adjustments, and employee balances         |

{% hint style="info" %}
**note:** CTO conversion is a different workflow. it creates time-off credit from eligible approved work. use **CTO Conversions**, the employee CTO balance, pool details, and transaction history instead of the ordinary leave conversion report.
{% endhint %}

\## generate a leave conversion report

1. confirm that the leave type is eligible for monetization and uses the intended conversion rule and schedule.
2. review pending applications, expired credits, adjustments, and the affected employee balances.
3. open **Reports → Leaves → Leave Conversion**.
4. click **Create New**.
5. enter the **Report Name**.
6. select the **Leave Type**.
7. choose **All** employees or **Employee Name**, then select the employee when required.
8. choose **Year** or **Specific Date** and complete the displayed period field.
9. create the report and open its details.
10. compare the report with the selected employees' balances and transaction ledgers before using the download.

when a balance correction changes the result, use the supported regenerate action and review the refreshed report. give the report a name that identifies its leave type and period.

### generate a forfeiture report

1. confirm that the leave type's unused-credit rule produces the intended forfeiture outcome.
2. review employee balances, pending requests, expiry, carryover, and adjustments.
3. open **Reports → Leaves → Forfeiture**.
4. click **Create New**.
5. enter the **Report Name** and select the **Leave Type**.
6. choose **All** employees or one employee.
7. choose **Year** or **Specific Date** and complete the period.
8. create the report and open its details.
9. compare the report with the affected employee transaction ledgers.

do not use a manual negative adjustment merely to make the report total match an expected amount. correct an incorrect employee transaction or leave rule through its supported workflow, then regenerate the report.

### why might a report differ from the current balance?

a saved report reflects the employee scope, leave type, and period used when it was generated. the current balance can change later because of an application, cancellation, expiry, carryover, conversion, import, transfer, or authorized adjustment.

check the report scope and generation date, then compare the employee transaction ledger. regenerate the report after correcting the source record when the supported action is available.

### related articles

* [configure leave settings](configure-leave-settings.md#page-066-pages-admin-leaves-leave-settings-md)
* [manage leave expiry, carryover, and conversion](manage-leave-expiry-carryover-and-conversion.md#page-067-pages-admin-leaves-leave-expiry-carryover-and-conversion-md)
* [trace leave transactions](../leave-requests-and-visibility/trace-leave-transactions.md#page-062-pages-admin-leaves-credits-and-related-workflows-leave-transaction-ledger-md)
* [manage compensatory time off](../balances-transfers-and-cto/manage-compensatory-time-off-cto.md#page-053-pages-admin-leaves-compensatory-time-off-md)
