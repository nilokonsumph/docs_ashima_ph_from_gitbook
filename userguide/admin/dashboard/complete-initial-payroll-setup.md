# complete initial payroll setup

Use **Dashboard Wizard** when an existing business needs the minimum payroll calendar and payroll-group structure required before its first pay run. The current wizard presents two guided steps: **Define Payroll Calendar** and **Choose or Create Payroll Group**.

**navigation:** go to **Dashboard**, then open **Dashboard Wizard**.

## before you begin

Complete the account-level work first:

1. create or choose the business in **Control Center**;
2. confirm that the administrator is assigned to the correct business; and
3. confirm that the administrator has access to the required Dashboard, Settings, Workforce, and Paycheck pages.

See [Control Center](../control-center/) for business and administrator access. The wizard configures payroll for the selected business; it does not create the business or grant administrator access.

## step 1: define payroll details

use **Define Payroll Calendar** to set the common working-day and working-hour basis and create the company's first payroll schedule.

1. enter the current payroll year.
2. enter the default working days in a year and normal working hours per day.
3. enable **Advanced Settings** only when ranks need different annual working-day values, then add the applicable rank rows.
4. choose the pay schedule. the current page supports **Semi Monthly**, **Fortnightly**, **Weekly**, and **Monthly** configurations when available to the company.
5. complete the applicable pay date, payroll period, cutoff, run-deadline, and non-working-day fields.
6. save and confirm that step 2 becomes available.

the schedule can govern a different employee population through its payroll group. a company can therefore maintain more than one payroll schedule after the initial setup when different employee groups are paid at different frequencies.

{% hint style="warning" %}
**warning:** annual working days and normal hours are calculation inputs. verify them before running payroll. use the complete **Pay Rate Calculation** and pay-schedule Settings articles when changing them after payroll activity exists.
{% endhint %}

## step 2: choose or create a payroll group

a payroll group connects employees who share a pay schedule and pay-calculation setup.

1. enter a clear payroll-group name.
2. choose the pay schedule created in step 1 or another available schedule.
3. choose the supported pay-calculation type and work schedule shown by the form.
4. add or update the group.
5. verify the saved group under **Settings → Paycheck → Pay Groups** before assigning employees or starting payroll.

create additional groups when employee populations use different schedules, work schedules, or supported calculation setups. the wizard starts the setup; the complete Settings pages remain the authoritative location for later maintenance.
