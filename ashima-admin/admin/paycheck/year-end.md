---
description: preparing your BIR Year-End using ashima
---

# Year end

<figure><img src="../../.gitbook/assets/Screenshot 2025-12-29 at 4.11.15 AM.png" alt=""><figcaption></figcaption></figure>

#### year-end process flow (at a glance)

When preparing for BIR year-end, Ashima guides you through the following key processes:

1. Run the Year-End / Perform Annualized Taxation / Finalize Withholding Tax Adjustments
2. Generate the Alphalist of Employees
3. Generate the DAT File for BIR Submission
4. Generate and Issue BIR Form 2316 for the year

Each step builds on the previous one. Completing them in order ensures that your payroll data, tax computations, and BIR submissions remain consistent and compliant.

### Accessing the Year-End Module

1. From the **top navigation bar**, click **Paycheck**.
2. Select **New Year End (Beta)**.

This opens the **Year-End dashboard**, where you will see:

* A list of **Draft Year-Ends**, grouped by **pay schedule**
* A table below showing **Approved** and **Rejected Year-Ends**

### Opening a Year-End Report

1. Locate the applicable **pay schedule**.
2. Click the **Year-End Report** for the target year.

If the report has not yet been generated, you will see a notice stating:

> **Data generation in progress**

### Generating the Year-End Report

If the Year-End Report has **not yet been generated**, click **Generate Year-End Report**.

#### Important Notes on Processing Time

* The **initial generation** or any **recalculation** requires processing time.
* Ashima gathers:
  * All **closed payrolls**
  * Uploaded payroll data (if any)
  * Employee records for the entire year
* **Please stay on the page and remain online** while processing is ongoing.

Once generation is complete, the report will automatically load.

#### What the Preparation of Year-End / Annual Payroll Report Entails

Ashima generates the **year-end payroll report** based on payroll data encoded and processed in the system. This report consolidates the employee’s annual payroll information, including:

* Total taxable and non-taxable compensation
* Statutory contributions
* Withholding taxes deducted during the year
* System-based adjustments and balances

**Client responsibility:**

* Review the report to confirm that all payroll entries are complete, accurate, and reflective of actual employee compensation
* Upload all previous employer 2316 of new employees
* Upload beginning balance, if any

Using the year-end report, the system performs **annualized taxation**, which recomputes the employee’s total income tax due for the year based on total annual taxable income.

This determines whether:

* There is **over-withholding** (subject to refund), or
* **Under-withholding** (requiring additional tax deduction)

**Client responsibility:**

* Review the annualized tax results
* Confirm that all income and deductions used in the computation are correct
* Approve the final tax figures before any adjustments are considered final

#### Final Tax Adjustments

Any tax differences resulting from annualization are reflected as **final withholding tax adjustments**, typically in the December payroll.

**Client responsibility:**

* Confirm that the final adjustments are valid and properly applied
* Ensure that each employee’s tax balance is correct before closing the year<br>

### Preparation of the Alphalist

Ashima prepares the **Alphalist of Employees** based on the finalized year-end payroll data in the system. This includes employee-level details such as compensation and taxes withheld.

**Client responsibility:**

* Review the Alphalist for accuracy and completeness
* Ensure that employee details, amounts, and classifications are correct and consistent with company records

***

###

## run the year-end in ashima (annualization & final tax calculation)

In Ashima, generating the **year-end report will** —

* run the annual payroll report,
* perform annualized taxation, and
* finalize withholding tax adjustments

are all completed by **running the Year-End module**.

This section walks you through **how to generate and review the Year-End Report** in Ashima.

### Accessing the Year-End Module

1. From the **top navigation bar**, click **Paycheck**.
2. Select **New Year End (Beta)**.

This opens the **Year-End dashboard**, where you will see:

* A list of **Draft Year-Ends**, grouped by **pay schedule**
* A table below showing **Approved** and **Rejected Year-Ends**

***

### Opening a Year-End Report

1. Locate the applicable **pay schedule**.
2. Click the **Year-End Report** for the target year.

If the report has not yet been generated, you will see a notice stating:

> **Data generation in progress**

***

### Generating the Year-End Report

If the Year-End Report has **not yet been generated**, click **Generate Year-End Report**.

#### Important Notes on Processing Time

* The **initial generation** or any **recalculation** requires processing time.
* Ashima gathers:
  * All **closed payrolls**
  * Uploaded payroll data (if any)
  * Employee records for the entire year
* **Please stay on the page and remain online** while processing is ongoing.

Once generation is complete, the report will automatically load.

***

### Reviewing the Generated Year-End Report

After generation, the report displays a list of employees under **two tabs**:

* **Above Minimum Wage (Above MWE)**
* **Minimum Wage Earners (MWE)**

All active and terminated employees are included and clearly tagged by employment status.

***

### Running “Check for Updates”

At the **top of the report table**, click **Check for Updates**.

This function validates and refreshes the report by performing the following checks:

* **Validates employee information**
  * Name
  * Employment status
  * MWE flag
  * TIN
* **Identifies late employees**
  * Employees not included during the initial run
* **Detects and flags duplicate TINs**

Click **Run Updates** to proceed.

***

### Navigating the Employee Table

#### Searching for an Employee

* Use the **search bar** to quickly locate a specific employee.

#### Viewing Payroll Period Details

* Click **Show Payroll Periods** to **hide or unhide**:
  * Closed payroll runs
  * Corresponding payroll amounts per period

This helps you focus either on totals or detailed breakdowns.

***

### Understanding How the Year-End Report Is Structured

The Year-End Report is arranged in logical sections from left to right:

#### 1. Payroll Data from Ashima

* Displays **taxable and non-taxable amounts**
* Sourced from **payrolls processed and closed in Ashima**

#### 2. Uploaded Beginning Balances (If Any)

* Shows taxable and non-taxable values from **uploaded beginning balances**
* Applicable if:
  * You started using Ashima **mid-year**
  * Earlier payrolls were processed outside Ashima

These values are added to ensure full-year totals are complete.

#### 3. Previous Employer 2316 Data

* Displays taxable and non-taxable amounts from **uploaded previous employer Form 2316**
* Applicable to **new hires within the year**

#### 4. Annualization and Final Tax Computation

* Totals all taxable income for the year
* Applies **annualized tax computation**
* Compares:
  * **Total tax due for the year**
  * **Total tax already withheld**

**Results:**

* If tax withheld is **greater** than tax due → **Refund**
* If tax withheld is **less** than tax due → **Payable**

These figures represent the **final year-end tax outcome** per employee.

***

### Reviewing the Draft Form 2316

* A **draft copy of Form 2316** is available within the Year-End Report.
* This allows you to review:
  * Compensation figures
  * Taxable vs non-taxable breakdown
  * Final tax amounts

> **Note:** This is still a **draft** and not yet the final issued Form 2316.
