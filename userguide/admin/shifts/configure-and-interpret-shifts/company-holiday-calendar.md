# maintain the company holiday calendar

## maintain the company holiday calendar

use the company holiday calendar to establish the holiday dates, types, locations, and rates that shifts, hours, and paycheck use for employee timekeeping and premium calculations.

**Navigation:**\
go to **Shifts → Holiday Schedule**.

{% hint style="warning" %}
a holiday-calendar change can recalculate affected timesheets and change open-payroll results. review the date, location scope, and rates before saving.
{% endhint %}

### why does the holiday calendar matter?

the holiday calendar tells Ashima:

* which date is a holiday;
* whether it is a regular holiday, special non-working holiday, or special working holiday;
* whether it applies to all locations or selected locations; and
* which unworked, worked, rest-day, overtime, and night-differential rates apply to that holiday row.

the general pay-rate tables provide default rate structures. the company holiday calendar stores the rates for each holiday and allows the company to review or set a different approved rate for that particular holiday.

### how do i review or download the calendar?

choose the **Year** view and use pagination to review its holidays. check each date, type, applicable locations, and rates. click a row to edit its details; use its checkbox when selecting it for deletion.

open the download menu and choose **excel** or **csv**. checkboxes do not limit this download.

{% hint style="warning" %}
the download does not follow the next-year view. check the dates in the exported file before using it as the next year's holiday list.
{% endhint %}

### how do i set up a new calendar year?

1. open **Shifts → Holiday Schedule** and select the required year.
2. when setup is offered, choose **Yes, I'm good with the default holiday schedule – let's roll!** to create the default calendar. wait for setup to finish.
3. if you prefer a custom list, choose **Nah, I want to upload my own custom holiday schedule.** this closes the setup prompt; it does not upload or save a calendar. follow [the import steps below](company-holiday-calendar.md#can-i-import-holidays).
4. review the saved holidays and permanent holidays. add missing proclamations, local holidays, and company-specific holidays.
5. check every holiday's type, date, location scope, and rates before payroll uses the calendar.

initialization copies the available parent/default holiday set and permanent holidays into the company year using the company's derived default rates. it is a starting point, not a substitute for the administrator's annual review.

at year-end or the start of a new year, initialize the next calendar and then add or correct holidays as official or company rules become available.

### how do i add a custom holiday?

1. select **Add Holiday**.
2. enter **Name** and **Date**. the datepicker allows 1 December of the previous year through 31 December of the current year. viewing the next-year list does not extend this range; use the import process for future-year dates outside the picker.
3. select **Type** and wait for its suggested company rates to load.
4. select the applicable locations, or leave the selection empty for all locations.
5. review the suggested rates. change only values covered by your company's approved rule.
6. if a **Double Holiday** notice appears, review the overlapping holidays and locations before saving. overlapping holiday rates are added together; correct an unintended overlap.
7. select **Save**, check the result, and confirm the holiday appears in the intended year. correct any required-field or save error before trying again.

choose **Cancel** or **X** to discard the unsaved holiday.

the supported business types are:

* **Regular Holiday**;
* **Special Non-Working Holiday**; and
* **Special Working Holiday**.

### how does location scope work?

no selected location means the holiday applies nationally or to all company locations. selected locations limit the holiday to employees assigned to those locations.

example: a city charter holiday can be created for the affected office location without applying it to employees assigned elsewhere.

location scope depends on the employee's assigned location. review employees with missing or outdated location assignments before relying on a local-holiday result.

you can create multiple custom holidays on the same calendar, each with its own applicable location group. do not create duplicate rows for the same employees and date unless the approved double-holiday rule requires separate holiday records.

### how do per-holiday rates work?

when a holiday type is selected, Ashima suggests the company's default rate group. the holiday row can store rates for:

* unworked monthly, daily, and hourly treatment;
* worked monthly, daily, and hourly treatment;
* worked rest-day treatment;
* rest-day overtime;
* ordinary overtime; and
* night differential.

this allows an approved custom holiday to use rates that differ from the general table. a custom rate is not automatically legally or contractually correct; it must come from the company's approved rule.

### how do i edit or delete a holiday?

#### edit a holiday

1. click the holiday row to open its details. clicking its checkbox selects it for deletion instead.
2. confirm **Name**, **Date**, and **Type**. **Type** is read-only in this form.
3. change the intended name, date, locations, or rates. the datepicker uses the same range as **Add Holiday**: 1 December of the previous year through 31 December of the current year.
4. review any **Double Holiday** notice and the affected locations before saving.
5. select **Save**, then reopen or review the refreshed record to confirm the result. use **Cancel** or **X** to discard the edit.

#### delete selected holidays

1. select the checkboxes for the holidays you intend to remove, then select **Delete**.
2. review the confirmation. if you need to check the dates or locations again, select **cancel** and review the selected rows.
3. select **delete** in the confirmation to remove the selected holidays.
4. check the result and refreshed calendar. review affected employee timesheets and open payroll.

holiday additions, edits, and deletions are recorded in the settings audit trail. review affected timekeeping and open payroll after a change; saving the calendar alone is not a final payroll review.

### can i import holidays?

use **Import holidays** when you need to add several holidays or future-year dates. the uploader opens in a new tab.

{% hint style="info" %}
import adds holidays; it does not edit or delete existing holidays. check for duplicates before uploading. **Upload File** checks and stages the file; **Continue** saves its valid rows.
{% endhint %}

#### prepare and upload the file

1. choose **Download Template** and keep its four headers unchanged.
2. complete each new holiday using the rules below. remove example rows and empty rows, then save as CSV.
3. choose **Browse File** and check the filename. remove a wrong selection before selecting the correct file.
4. choose **Upload File** and review the validation result.

| column                   | what to enter                                                                                                                                       |
| ------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Holiday Name**         | the holiday name; required.                                                                                                                         |
| **Holiday Date**         | a date in the current or a future year, in **dd-MMM-yy** format, such as **31-Jan-27**; required.                                                   |
| **Holiday Type**         | **Regular Holiday**, **Special Non-Working Holiday**, or **Special Working Holiday**, using the template's accepted values; required.               |
| **Applicable Locations** | leave blank for all locations. for specific locations, use their exact configured names separated by a vertical bar, for example `Cebu \| Mandaue`. |

#### review and save the valid rows

1. read every validation error. to correct the file before saving anything, choose **Retry**, correct the CSV, and upload it again. **Retry** discards the staged file.
2. if at least one valid row exists, **Continue** is available. decide whether to save those valid rows now or correct the complete file first.
3. choose **Continue** to save the valid rows, including when there are no errors.
4. check the result, then review the saved names, dates, types, locations, and rates in the company calendar.

{% hint style="warning" %}
when you continue with errors, invalid rows are skipped. after correcting those rows, upload only the holidays still missing from the calendar so you do not add the successful rows again.
{% endhint %}

### annual review checklist

* correct year initialized;
* national and permanent holidays present;
* official updates and proclamations added;
* company-specific holidays added;
* local holidays limited to the correct locations;
* holiday types correct;
* custom rates approved and reviewed;
* no unintended duplicate or double-holiday rows;
* employee locations current; and
* affected timesheets and open payroll reviewed.

### related articles

* [shift calendar and overview](../plan-and-assign-shifts/shift-calendar-and-overview.md#page-033-pages-admin-shifts-shift-calendar-and-overview-md)
* [rest days and shift enforcement](rest-days-and-shift-enforcement.md#page-042-pages-admin-shifts-rest-days-and-shift-enforcement-md)
* [hours: rest-day and holiday work](../../hours/)
* [holiday and rest-day settings](../../settings/time-entry-hours-shifts-and-holidays/configure-holidays-and-the-holiday-calendar.md)
