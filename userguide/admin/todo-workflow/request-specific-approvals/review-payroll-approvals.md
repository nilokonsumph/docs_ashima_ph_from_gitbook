# review payroll approvals

## review payroll approvals

use **Todo → Payroll** to review a submitted pay run before it advances to its next controlled status.

### review the pay run

confirm the company, payroll group, coverage period, pay date, employee count, included and excluded employees, recalculation state, source warnings, total net pay, payroll masterlist, material employee details, and ingestion entries. the Payroll approval detail provides the payroll masterlist; do not expect the bank file from this approval page.

### approve or reject a pay run

1. open the submitted pay run.
2. review the summary and warnings.
3. open the payroll masterlist and material employee details.
4. confirm that source changes have been recalculated.
5. select the available approval or rejection action.
6. enter the password requested by the confirmation.
7. confirm, then verify the resulting pay-run status.

{% hint style="warning" %}
**warning:** payroll approval can lock a critical processing stage. correct and recalculate the source before approval. if Payroll Lock is configured to suspend administrator To Do approvals, the applicable approval actions remain restricted while that lock condition applies.
{% endhint %}
