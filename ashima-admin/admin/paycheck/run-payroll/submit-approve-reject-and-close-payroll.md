# Submit, approve, reject, and close payroll

use **Submit for Approval** only after the open pay run is recalculated, reviewed, and ready for the configured Payroll approval workflow.

**Navigation:**\
go to **Paycheck → Pay Run → Payroll**, then open **View Payroll Masterlist** for the open pay run.

## before submission

1. review the payroll masterlist and Employee Pay Details.
2. resolve exclusions and approved adjustments.
3. select **Check for Pay Updates**.
4. recalculate employees with timesheet, shift, setting, or pay-item updates.
5. confirm that the payroll readiness indicators no longer block submission.
6. review the pay date, period, employee count, totals, and negative net pay results.

**Submit for Approval** remains unavailable while the current readiness checks require correction or recalculation.

## what happens after submission?

the pay run leaves normal open-payroll preparation and follows the configured Payroll workflow. Assigned approvers review the request from the Payroll queue in **Todo**. The displayed approval level, approver, decision, and date form the payroll's approval evidence.

* approval advances the configured workflow and, after the final required approval, closes the payroll;
* rejection returns the payroll for correction according to the current workflow; and
* a waiting or closed payroll should not be treated as an editable open draft.

## what changes after payroll is closed?

the closed masterlist removes open-preparation actions and exposes payment and payslip outputs such as **Download Bank File**, **Print Payslip**, and the payslip generation control. In Ashima, closing is the end of the payroll calculation and approval lifecycle; it is treated as paid for product workflow purposes even though Ashima does not verify external bank receipt.

## rules and warnings

* approval behavior depends on **Settings → Workflow → Workflow Task Settings** for Payroll.
* assignment to an approver and permission to view confidential payroll data are separate controls that must both be valid.
* do not close a payroll merely to test an output. Use an approved test payroll or a planned end-to-end test with recorded cleanup and expected downstream effects.

## related articles

* [payroll masterlist and readiness](/broken/pages/90993c9dd2e7045a5799c0b820706e27adc169e8)
* [payroll exclusions](/broken/pages/73f5b6a6bf0e9a1ffaa726d943f78e7ccd120cac)
* [payslip output](/broken/pages/c2006cb19c802e2f80eb98c994a9d170683e417d)
