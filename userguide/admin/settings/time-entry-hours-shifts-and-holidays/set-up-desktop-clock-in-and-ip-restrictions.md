# set up desktop clock-in and IP restrictions

to enable desktop clock in turn ON the settings under **settings > hours > time entry > desktop clock in**

when employees log in to their ashima employee portal, a timeclock is displayed along with the corresponding **Time In** and **Time Out** buttons. this is the default method of recording work hours.

you can further secure or customize this process by enabling features such as photo capture and IP restrictions.

## how does photo capture work?

* this feature captures an employee’s photo when they clock in or out from their desktop portal.
* a webcam must be connected to the employee’s device.
* photos are stored with the timesheet record for reference.

{% hint style="info" %}
**note:** If photo capture is enabled, employees need a working desktop webcam and must complete the photo step before the time log is accepted.
{% endhint %}

## how does IP restriction work for desktop clock-in?

* when enabled IP restriction ensures employees can only clock in or out from **company-approved IP addresses**.
* this requires static IP addresses for your office networks.
* to easily manage your IP addresses especially if you have multiple IP addresses assigned to multiple locations start by defining/creating IP locations on your location settings.
  * first, go to **settings > workforce > location & worksites** and add the IP locations you want to define.

when creating a new location make sure to choose IP location on the drop down on where to use this for.

* next, on the **settings > hours > time entry>desktop clock in** add the IP addresses you want to be part of your white list.
* on the time entry settings, if you add any IP location, the whitelist applies **globally** to all employees. all your employees will be able to clock in from the company-wide trusted IP addresses.

{% hint style="info" %}
**note:** use this feature if you want to limit desktop clock-ins strictly to your company’s networks.
{% endhint %}

## can i enable IP restriction for specific employees?

* if you want certain employees to clock in only from specific IPs (that other employees cannot use), you can by enabling IP restriction to **employee level**
* to configure this go to the individual employee workforce profile, and click on employee’s **time entry settings**, switch on **employee-level IP restriction**.
* add the specific IP address(es) you want to limit for that employee, choose the location you created to help you define the custom IP you assigned to this employee.
* Once applied, the employee will only be able to clock in/out from the assigned IP address(es).

## can i whitelist multiple IP addresses?

yes. if you need to whitelist more than one IP address, you can either:

* add them individually to the trusted IP list, or
* **upload multiple IPs** at once using the IP upload for faster setup.

## verify desktop access

1. save the desktop clock-in option and approved IP addresses.
2. test from one approved network and confirm that the clock action and resulting time log are available.
3. test the intended restriction boundary from a non-approved network when company policy permits.
4. if access is wrong, correct the approved IP entry and location mapping, save again, and repeat the controlled test.

## continue in the affected module

* [review captured time and timesheets](../../hours/)
