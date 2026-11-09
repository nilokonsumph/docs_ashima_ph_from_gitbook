# start here: understand Paycheck

## start here: understand Paycheck

the **Paycheck** module is where administrators create, review, and manage payroll runs in the Admin Portal.

use this module to move payroll from draft pay run through approval, payment processing, and payslip release. the module also gives access to the earnings, deductions, contribution, and withholding tax pages that support payroll calculations.

payroll in Ashima follows three stages:

1. **payroll input** — create the pay run, review employee-level payroll values and recalculate if needed.
2. **preview & approve** — review the consolidated payroll output (masterlist), exclusions, adjustments, and approval readiness.
3. **process payment** — handle bank file output, payslip generation, and payslip release after payroll is closed.

### how is this guide organized?

The Paycheck guide follows the major payroll functions rather than presenting one long list of pages:

* [run payroll](run-payroll/) — regular payroll from draft through closing and payslip release;
* [corrections, controls, and ingestion](corrections-controls-and-ingestion/) — current and late corrections, imports, Payroll Lock, and supporting utilities;
* [pay items, contributions, and tax](pay-items-contributions-and-tax/) — trace payroll inputs and statutory results;
* [salary increases and retroactive pay](salary-increases-and-retroactive-pay/) — individual or bulk salary changes and supported prior-period differences;
* special payroll processes — 13th Month, termination, maternity, and Year End;
* [Projection Tool](use-projection-tool-v2.md) — optional annual withholding-tax estimates and supported adjustments; and
* [disbursement](disbursement/) — supported payment preparation, approval, and outputs.

The guide categories do not replace the exact Admin Portal navigation shown inside each task. They help you find the correct end-to-end workflow even when one workflow uses Paycheck, Settings, Reports, To Do, Upload Manager, or Utilities pages.

### what pages are available in the Paycheck module?

The current Admin Portal groups the main **Paycheck** menu into **Pay Run**, **Earnings**, **Deductions**, and **Contributions**, followed by **Withholding Tax**. The pages shown to an administrator can depend on role privileges and company configuration.

| menu group        | page                   | what you use it for                                                      |
| ----------------- | ---------------------- | ------------------------------------------------------------------------ |
| **Pay Run**       | **Payroll**            | create, calculate, review, approve, close, and release payroll           |
| **Pay Run**       | **Year-End**           | prepare and review annual payroll and tax output                         |
| **Pay Run**       | **Paycheck Surfacing** | investigate employee payroll evidence and related source records         |
| **Pay Run**       | **Payroll Lock**       | pause covered payroll-sensitive changes while payroll is being finalized |
| **Earnings**      | **Compensation**       | review and maintain employee compensation records                        |
| **Earnings**      | **Allowances**         | configure and assign allowance earnings                                  |
| **Earnings**      | **De Minimis**         | configure and assign De Minimis benefits                                 |
| **Earnings**      | **13th Month**         | calculate and review 13th Month payroll                                  |
| **Earnings**      | **Other Earnings**     | configure and assign other earning types                                 |
| **Earnings**      | **Beginning Balance**  | record prior payroll balances needed for payroll and annual reporting    |
| **Earnings**      | **Previous 2316**      | record previous-employer tax information                                 |
| **Earnings**      | **Retroactive Pay**    | review salary differences carried from earlier periods                   |
| **Deductions**    | **Government Loans**   | maintain employee government-loan deductions                             |
| **Deductions**    | **3rd Party Loans**    | maintain employee third-party-loan deductions                            |
| **Deductions**    | **Other Deductions**   | maintain company-defined deduction assignments                           |
| **Deductions**    | **Insurance**          | maintain employee insurance deductions                                   |
| **Contributions** | **SSS Contribution**   | review employee SSS contribution records                                 |
| **Contributions** | **HDMF Contribution**  | review employee HDMF contribution records                                |
| **Contributions** | **PHIC Contribution**  | review employee PhilHealth contribution records                          |
| **Contributions** | **SSS Rules**          | review the SSS contribution rules used by payroll                        |
| **Contributions** | **PHIC Rules**         | review the PhilHealth contribution rules used by payroll                 |
| **Contributions** | **HDMF I Rules**       | review regular HDMF contribution rules                                   |
| **Contributions** | **HDMF II Rules**      | review modified or additional HDMF contribution rules                    |
| —                 | **Withholding Tax**    | review withholding-tax payroll output                                    |

#### which related payroll pages are outside the Paycheck menu?

Some payroll work starts in another main menu. Use the page that matches the task instead of looking for a generic **Pay Run Tools** page.

| area                   | payroll-related pages available in the current Admin Portal                                                                                                          |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Settings → Pay Run** | **Pay Schedule**, **Pay Rate Calculation**, **Pay Rates (by Date Type)**, **Pay Groups**, **Payment Options**, **Payslip Template**, and **Post Payroll Adjustment** |
| **Settings**           | payroll tax and compliance tables; earning, deduction, contribution, and withholding-tax rules                                                                       |
| **Upload Manager**     | earning and deduction imports plus **Payroll Exclusion**, **Payroll Withholding Tax Adjustment**, and **WT Fixed**                                                   |
| **Reports → Pay Run**  | **Payroll Register**, **Accounting Entries**, **Cost Structure**, and **Compensation History**                                                                       |
| **Reports**            | tax, SSS, PhilHealth, HDMF, audit, and other supported payroll reports                                                                                               |
| **Utilities**          | **Disbursement** for supported payment-processing work                                                                                                               |

{% hint style="info" %}
The Paycheck guide connects the complete payroll workflow. Field-level Settings procedures, report generation, and general approval mechanics remain owned by their respective guide sections even when Paycheck links to them.
{% endhint %}

use this section to create, calculate, review, approve, close, and release a regular pay run.

**Navigation:**\
go to **Paycheck → Run payroll**.

### recommended order

1. open **Pay run workspace and history**.
2. use **Create or delete a draft pay run**.
3. review and recalculate the draft.
4. inspect **Employee pay details** for exceptions.
5. complete **Payroll masterlist and readiness** checks.
6. review exclusions and send a pay draft when required.
7. submit, approve, reject, and close payroll.
8. release or download the approved payslip output.

complete source corrections and recalculation before approval. In Ashima, closing is the end of the payroll workflow and completed payroll is treated as paid for platform processing.

use this section to manage payroll locks, adjustments, ingestion, post-payroll adjustments, imports, payroll-group transfers, and investigation tools.

**Navigation:**\
go to **Paycheck → Corrections, controls, and utilities**.

### choose the correct page

* use **Payroll lock** for payroll-sensitive employee and manager actions;
* use **Paycheck adjustments and ingestion** for eligible open-run entries;
* use **Post-payroll adjustments** for supported late changes;
* use **Beginning balances and imports** for approved bulk inputs;
* use **Payroll-group transfer** for eligible employee movement; and
* use **Paycheck surfacing** to investigate related evidence before changing a source.

these tools have different audit and recalculation effects. Do not use an adjustment when the underlying source record can still be corrected through its normal workflow.

use this section to review earnings, deductions, contributions, withholding tax, de minimis, and employee payroll treatment.

**Navigation:**\
go to **Paycheck → Pay items and statutory review**.

### recommended approach

1. review the company item or statutory setting.
2. confirm the employee assignment or entitlement.
3. review the applicable pay dates and schedule.
4. calculate or recalculate the open payroll.
5. inspect Employee Pay Details and Payroll Register output.

setup, employee assignment, and payroll result are separate layers. A configured item does not affect an employee until the applicable assignment and payroll conditions are met.

### salary increase

use salary increase to record a new basic pay and the date when it starts, whether the change applies now, in a future payroll period, or to payroll periods already processed.

{% hint style="warning" %}
a salary increase changes payroll calculations. review the new basic pay, effective date, and employee entitlements before you proceed. recalculate any affected open pay run before relying on the result.
{% endhint %}

### how does salary increase work?

you enter the employee's new basic pay and effective date. Ashima records the change in compensation history, then uses the effective date to determine how the change applies.

| effective date                            | what happens                                                                                                                 |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| inside the current payroll period         | the current payroll uses the applicable old and new rates; salary increase details explain the calculation                   |
| inside a payroll period already processed | Ashima calculates the unpaid difference as retroactive pay when retroactive pay is enabled                                   |
| inside a future payroll period            | the current basic pay remains in use until the effective date; the new basic pay applies when the future period is processed |

you do not select a current, future, or retroactive mode. the effective date controls the result.

### how can I initiate a salary increase?

use either of these workflows:

* increase one employee's salary — update one employee from the compensation page.
* update salaries in bulk — upload salary changes for up to 50 employees at a time through **Retroactive Pay Import**.

### where is the change recorded?

Ashima adds the change to the employee's compensation history. the history identifies the previous basic pay, new basic pay, effective date, adjustment date, details, and the person who processed the change.

use compensation history to confirm that the salary record and effective date were saved correctly before processing payroll.

### where can I review the payroll result?

for an increase inside the current payroll period, open the employee's pay details and review salary increase details.

for an increase that affects payroll periods already processed, review the generated amount in retroactive pay.

### what settings affect the result?

* the employee's pay rate, pay schedule, assigned shift, attendance, and effective date determine how regular pay is calculated.
* **Retroactive Pay** must be enabled under paycheck earnings settings before Ashima calculates a past-period salary difference.
* an affected open pay run must be recalculated to include the latest compensation change.

### related articles

* increase one employee's salary
* update salaries in bulk
* salary increase details
* retroactive pay

***

**Navigation:**\
go to **Paycheck → Special payroll workflows**.

### choose the correct workflow

* **13th Month:** calculate, review, adjust, approve, and produce 13th Month output.
* **Termination and final pay:** prepare final-pay components and employee separation output.
* **Maternity benefits:** review benefit, reimbursement, payroll, and return-to-work treatment.
* **Year End:** review annual payroll and tax information and produce supported year-end outputs.

each workflow has its own settings, recalculation, approval, and reporting requirements. Do not treat one special-payroll result as a substitute for another.
