# configure Paycheck before running payroll

## configure Paycheck before running payroll

Paycheck calculations depend on configuration and employee records that sit outside the main **Paycheck** menu. Review these controls before the first payroll and whenever the expected result differs from the calculated result.

{% hint style="warning" %}
Changing a setting or source record does not by itself prove that an existing payroll result has changed. If the affected pay run is still eligible for recalculation, recalculate it and review the employee result again. Submitted or closed payroll follows its available correction workflow instead of the normal open-run edit path.
{% endhint %}

### which configuration should I review first?

Use **Settings → Pay Run** for the payroll backbone.

| setting                      | what it controls or supplies                                                                        | what to verify                                                                               |
| ---------------------------- | --------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| **Pay Schedule**             | the payroll frequency and period structure available to payroll groups                              | the schedule matches when the group is paid                                                  |
| **Pay Rate Calculation**     | the payroll calendar and calculation basis used with employee pay-rate records                      | the calendar and calculation method match the company's intended payroll treatment           |
| **Pay Rates (by Date Type)** | rate treatment for supported date types, such as regular work, holidays, or rest days               | the current date-type rates are appropriate before relying on calculated earnings            |
| **Pay Groups**               | which employees are processed together and which pay schedule applies                               | the employee belongs to the correct group and the group has the intended schedule            |
| **Payment Options**          | supported company payment and bank-output configuration                                             | the intended payment option is available before payment processing                           |
| **Payslip Template**         | the presentation and supported content of generated payslips                                        | the current template is appropriate before payslips are released                             |
| **Post Payroll Adjustment**  | whether supported PPA workflows are available and how far back an eligible correction may be raised | PPA is enabled when required and the configured previous-payroll limit covers the correction |

An employee's compensation, pay-rate type, payroll group, work schedule, and applicable assignments must also be correct. Company settings provide rules; employee records determine which of those rules and values apply to a person.

### how does Pay Rate Calculation affect payroll?

**Pay Rate Calculation** supplies the payroll-year and work-time basis used to derive daily and hourly reference rates from a monthly salary. It does not replace the employee's saved compensation record.

| setting                           | what it controls                                                                  | what to watch for                                                                                            |
| --------------------------------- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Payroll Year**                  | the standard number of working days used for the monthly-to-daily rate conversion | the selected calendar basis must match company policy; changing it can change derived daily and hourly rates |
| **Average Working Hours Per Day** | the divisor used when a daily reference rate must be expressed as an hourly rate  | use the normal workday expected by company policy and the applicable employment rules                        |
| **Enable Advanced Settings**      | allows a different total working-days value for each employee rank                | a rank-specific value takes the place of the single company value for employees in that rank                 |

For a monthly-paid employee, the guide uses this relationship when the configured calendar basis applies:

> **Daily reference rate = monthly salary × 12 ÷ configured working days in the payroll year** **Hourly reference rate = daily reference rate ÷ configured average working hours per day**

For example, a monthly salary of PHP 26,100 with 261 working days and 8 working hours per day produces a PHP 1,200 daily reference rate and a PHP 150 hourly reference rate. Use the actual employee record and company settings for payroll review; the example is a reading aid, not a substitute for the calculated breakdown.

{% hint style="warning" %}
Do not change the payroll-year basis only to make one employee's result match an expected amount. First confirm the employee's pay type, rank, compensation effective date, payroll group, and time inputs. After an authorized setting change, recalculate an eligible open pay run and compare the employee's daily or hourly breakdown before and after the change.
{% endhint %}

### how do Pay Rates (by Date Type) work?

**Pay Rates (by Date Type)** determines how eligible work or non-work on each supported date type is credited. The table separates base treatment from add-on treatment:

* the **not working**, **working**, and **rest day** columns control the base multiplier for the employee's pay type and date context;
* the **overtime** and **night shift differential** columns control add-on multipliers applied when the matching hours qualify; and
* an employee-level night-differential restriction can limit that add-on for selected employees when the option is enabled.

A value of **0** means no credit under that cell's condition. A value of **1** represents one base unit. A value above **1** applies the configured premium. For monthly-paid employees, a value of **1** in a non-working cell normally preserves the salary treatment for that date; for daily- or hourly-paid employees, the same date can use a different configured value. This is why the table must be read by date type, work state, and pay type together.

{% hint style="warning" %}
These values affect payroll calculations and must follow the company's authorized payroll policy and applicable law. Treat the values shown in a test tenant as evidence of the interface, not as universal statutory advice. After a change, recalculate a safe open-payroll example for each affected pay type and verify the regular, holiday or rest-day, overtime, and night-differential lines separately.
{% endhint %}

### how do Pay Schedules work?

A **Pay Schedule** defines how often employees are paid and supplies the pay-period and pay-date framework used by a payroll group. A company can maintain more than one frequency at the same time. For example, one payroll group can use **Semi Monthly** while another uses **Weekly**, **Fortnightly**, or **Monthly**.

| frequency        | meaning                                                        | common result                                 |
| ---------------- | -------------------------------------------------------------- | --------------------------------------------- |
| **Monthly**      | one payroll cycle each month on the configured monthly pay day | 12 scheduled pay days in a full year          |
| **Semi Monthly** | two payroll cycles each month on the two configured pay days   | normally 24 scheduled pay days in a full year |
| **Weekly**       | one payroll cycle each week on the configured weekday          | a weekly sequence of pay dates                |
| **Fortnightly**  | one payroll cycle every two weeks on the configured weekday    | an every-other-week sequence of pay dates     |

Each payroll group selects one available Pay Schedule. The company can therefore run different employee populations on different frequencies without treating one schedule as the company-wide schedule for everyone.

The schedule also records the cutoff or covered period, first pay date, payroll-run deadline, and what to do when a pay date falls on a non-working day. The available choices are **Same Day**, **Move To Next Working Day**, and **Move To Previous Working Day**.

{% hint style="warning" %}
Review the generated pay calendar before processing payroll. The current page warns that processed pay-period dates cannot simply be changed and that changing periods after pay runs have been processed can cause year-end discrepancies.
{% endhint %}

### why are Pay Groups important?

A **Pay Group** is a payroll-processing definition, not only a list or filter. It groups employees who are processed together and supplies defaults that Paycheck and timekeeping use later. Pay runs are created per payroll group, so a group affects which employees appear together, the available pay dates, how their basic pay is interpreted, and the work schedule used as the starting point.

| Pay Group field               | purpose                                                                   | downstream effect                                                                                   |
| ----------------------------- | ------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **Payroll Group Name**        | identifies the employee population                                        | becomes available for employee assignment and pay-run selection                                     |
| **Payroll Group Description** | records the business meaning of the group                                 | helps administrators distinguish groups with similar names or schedules                             |
| **Pay Schedule**              | selects the group's Monthly, Semi Monthly, Weekly, or Fortnightly cadence | controls the pay calendar and available payroll periods for that group                              |
| **Pay Calculation Type**      | selects **By Month**, **By Day**, or **By Hour**                          | supplies the default rate interpretation used for employees assigned to the group                   |
| **Assigned Work Schedule**    | selects the group's starting work schedule                                | becomes the default schedule resolved from the payroll group for assigned employees and timekeeping |
| **Confidential**              | marks the group as a confidential payroll population                      | restricts the group and its employees to the matching confidential-access scope                     |

#### how many employees can a Pay Group contain?

Plan for a maximum of **150 employees in one Pay Group**. When a group reaches that size, create another Pay Group with the appropriate Pay Schedule, Pay Calculation Type, and Assigned Work Schedule, then assign the additional employees to it.

The Pay Group limit is separate from the total number of employees allowed by the company's subscription. Both rules can affect whether another employee can be added or moved.

#### how does Assigned Work Schedule act as a default?

The selected work schedule is stored on the payroll group. When an employee is assigned to that group, Ashima uses the group's schedule as the default schedule context. That is why the Pay Groups list displays **Assigned Work Schedule** beside each group.

An authorized administrator can later assign a different dated employee shift or schedule through the applicable Shifts workflow. That employee-level change does not redefine the Pay Group default for everyone else. Before changing a group default, review the employees already assigned to the group and the open time or payroll periods that may use it.

#### what does Confidential do?

Selecting **Confidential** classifies the Pay Group as a confidential payroll group. It is an access and population boundary:

* confidential employees must use a payroll group with the same confidential status;
* non-confidential employees use non-confidential groups;
* available payroll groups and employee/payroll records are filtered according to the administrator's confidential-access scope; and
* changing an employee's confidential status or group can be blocked while that employee is included in an open pay run.

Do not use **Confidential** as a general label for a sensitive department. Enable it only when the employee population must follow Ashima's confidential payroll-access workflow, and confirm that the administrators who must process the group have the matching access.

### which configurable rules affect earnings, deductions, contributions, and tax?

| Settings area     | examples in the current Admin Portal                                                                         | effect on payroll                                                                                         |
| ----------------- | ------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| **Earnings**      | **Allowance**, **De Minimis**, **13th Month**, **Hazardous Pay**, **Other Earning**, and **Retroactive Pay** | defines supported earning behavior, limits, or options before employee assignment and payroll calculation |
| **Deductions**    | **Government Loans**, **Third Party Loans**, **Insurance**, and **Other Deductions**                         | defines supported deduction behavior before employee assignment and payroll calculation                   |
| **Contributions** | **Contribution Calculation**, **Contribution Schedule**, and **Contribution Rules**                          | controls supported contribution method, timing, and rule choices                                          |
| **Taxes**         | **Withholding Tax Deduction Schedule** and **Withholding Tax Contribution Rules**                            | controls supported withholding-tax timing and rule choices                                                |

Use the detailed Settings guide for field-level setup. In this Paycheck guide, each workflow identifies the setting or employee record that can change its result.

#### how do I configure Hazardous Pay?

Use **Settings → Earnings → Hazardous Pay** to enable the feature and create reusable Hazardous Pay definitions.

| choice                                            | effect                                                                                                                |
| ------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| **Frequency: Per Workday**                        | evaluates the configured benefit by eligible workday                                                                  |
| **Frequency: Hours Worked**                       | evaluates it from qualifying hours and requires the applicable hours range                                            |
| **Variability Type: Daily Rate Percentage**       | calculates the benefit from the configured percentage of the applicable daily rate                                    |
| **Variability Type: Specific Amount**             | uses the configured fixed amount                                                                                      |
| **Rank**, **Employment Status**, and **Position** | define which employee populations can qualify; the form requires at least one targeting basis                         |
| **Tax Exempt**                                    | records whether the Hazardous Pay definition is treated as exempt or not exempt in the supported payroll and tax flow |
| **Entitled even when employee absent**            | allows the definition to remain eligible under the supported absence condition                                        |
| **Entitled even when employee on leave**          | allows the definition to remain eligible under the supported leave condition                                          |
| **Requirements** and **Note**                     | record supporting conditions and administrator context                                                                |

Enabling the feature or saving a definition does not by itself prove that every employee has earned the amount. The employee must match the configured population and the applicable payroll input must qualify. After setup, recalculate a safe open pay run, confirm the **Hazard Pay** earning line for an eligible and an ineligible employee, and verify the intended tax treatment on the payroll breakdown.

#### what are Payroll Tax & Compliance Tables?

**SSS**, **PhilHealth**, **HDMF**, and **Withholding Tax** under **Payroll Tax & Compliance Tables** are governed statutory reference views. They are not ordinary company preferences and the current Admin pages do not provide an administrator save action for editing the tables.

| reference table     | what it supplies to the applicable calculation or review                                                                                                           |
| ------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **SSS**             | compensation brackets, Monthly Salary Credit, employee and employer Social Security shares, EC, Mandatory Provident Fund, and totals for each published table year |
| **PhilHealth**      | the active compensation or premium basis and employee/employer share used by the supported PhilHealth calculation                                                  |
| **HDMF**            | the active compensation ranges, rates, and employee/employer share used by the supported HDMF calculation                                                          |
| **Withholding Tax** | annual compensation brackets and the fixed-plus-percentage basis used by the supported annual withholding-tax reference                                            |

The SSS page can display more than one published table year. The calculation service selects the applicable governed data; merely viewing an older table does not make it active. When a statutory rule changes, it must enter Ashima through the authorized product/reference-data process and be validated against its effective period.

To verify a governed-table update, use safe employees below, within, and above a changed bracket; recalculate an eligible open pay run; compare employee and employer shares or withholding; and confirm that closed historical payroll remains governed by its supported correction process. Do not overwrite an employee result manually to simulate a statutory-table update.

### which settings control payroll approval and visibility?

**Workflow Task Settings** and **Manager Access Settings** belong to the approval and access layer. They do not calculate an earning, deduction, contribution, or tax amount.

#### how does the Payroll workflow affect Paycheck?

In **Workflow Task Settings**, the **Payroll** workflow defines the approval group, approval levels, approvers, notification channel, and whether staff receive a notification. Payroll uses a global workflow: creating a new Payroll workflow replaces the current workflow assigned across the company rather than requiring employee-by-employee assignment.

{% hint style="warning" %}
Before replacing the Payroll workflow, clear or resolve pending items that still depend on the current approvers. A replacement changes the route used by later supported submissions; it does not recalculate payroll amounts or safely migrate unfinished approval work by itself.
{% endhint %}

After configuration, submit only an approved test payroll when validation is required. Confirm that the intended approver receives the item in **Todo**, that each approval level advances in order, and that the Payroll Masterlist shows the matching approval status.

#### does Manager Access change payroll calculation or approval?

No. **Manager Access Settings** defines the employees a manager can see and the module actions the manager can perform, such as view, add, edit, or delete within supported team workflows. Visibility can be scoped to direct reports or selected departments, with the configured direct-to or department targets.

Manager Access does not grant the Admin Paycheck calculation privilege and does not replace the Payroll approval workflow. It can affect who may work with upstream Hours, Leave, Overtime, Shifts, or Workforce records that later feed payroll. Test the result while signed in as the intended manager: verify both the employee population and the allowed actions, then confirm that a restricted employee or action is absent.

### how do imports feed Paycheck?

Use **Upload Manager** when a supported bulk file is the appropriate source. Payroll-related imports include earnings and deductions plus **Payroll Exclusion**, **Payroll Withholding Tax Adjustment**, and **WT Fixed**. The current portal also provides supported imports for beginning balances, previous 2316 information, bank information, overtime fixed rates, workflow approvals, and disbursement.

An uploaded file is an input, not proof of the final payroll result. Review the import outcome, recalculate the eligible open pay run when required, and verify the affected employees on **Pay Run Details** or the **Payroll Masterlist**.

### which settings control payment and payslip output?

#### what do Payment Options control?

**Payment Options** configures the supported bank-file layout for the company. Select the bank and enter the bank-assigned company code plus any bank-specific fields, such as branch, funding-account, or payroll-branch codes. The available fields depend on the selected bank.

This setting does not assign an employee's bank account and does not change net pay. Configure it before generating the applicable bank or disbursement output, follow the bank's current implementation instructions, then review a safe test file for layout, company identifiers, totals, and employee count before using the output operationally.

#### what does the Payslip Template control?

**Payslip Template** controls presentation. It can show or hide supported earnings and deductions, nested detail lines, government-loan and third-party-deduction summaries, employee details, company logo and address, primary contact email, and a custom footnote. Print options can also control whether an item appears in the two-payslip or four-payslip layout.

Hiding a line does not remove the earning or deduction from payroll and does not recalculate the employee's net pay. Review the template before payslips are released. After a change, preview a safe generated payslip in the web view and every intended print layout; verify totals, child detail lines, company details, contact information, and the custom footnote.

### where do approvals, reports, and payment output appear?

* **Todo** can show payroll and related approval work when the signed-in user, workflow, and record state make an action available.
* **Reports → Pay Run** provides **Payroll Register**, **Accounting Entries**, **Cost Structure**, and **Compensation History**.
* Other report groups provide supported tax, SSS, PhilHealth, HDMF, BIR, audit, and log outputs.
* **Settings → Report → Payroll Journal Entries** maps supported earning, government-contribution, and other-deduction categories to account codes and descriptions used by **Accounting Entries** output. The same generic account may be used for more than one category when that matches company accounting policy. This mapping does not determine employee payroll amounts. Configure it before report generation, then regenerate or reopen a safe Accounting Entries output and verify the mapped accounts, debit/credit presentation, and payroll totals.
* **Utilities → Disbursement** supports the applicable payment-processing workflow after payroll review.
* Generated employee payslips are a separate closed-payroll output and must be generated and reviewed before release.

### what upstream records can change payroll?

Paycheck consumes eligible data from **Workforce**, **Hours**, **Leaves**, and **Shifts**. This can include employment and compensation details, payroll-group membership, time records, overtime, leave, schedules, holidays, earnings, deductions, contributions, and tax information. Correct the owning record first, then recalculate and review the open pay run when the workflow permits.

{% hint style="info" %}
Visibility is conditional. If a page or action described here is missing, check the user's role and privileges, the company configuration, the employee or payroll state, and whether the feature applies to that record.
{% endhint %}
