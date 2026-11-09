# manage employee and administrator 2FA

use this guide to manage company-level employee 2fa in ashima. this includes turning the feature on, reviewing **Admin 2FA Enforcement**, reviewing who has completed setup, and resetting 2fa for employees who are fully locked out.

the main workflow is:

1. turn on **Two-Factor Authentication Feature** so employees can set up 2fa.
2. review or update **Admin 2FA Enforcement** if 2fa should be required for admins.
3. use **Employee 2fa Status** to review setup status and reset 2fa when needed.

## **what is two-factor authentication (2fa)?**

two-factor authentication adds an extra layer of security by requiring two verification steps during login. even if someone knows a user’s password, they cannot access the account without the authentication code from the user’s device.

ashima uses app-based 2fa, which allows employees to use **any trusted authenticator app they already use or prefer**, such as google authenticator, microsoft authenticator, or other compatible authenticator tools.

these apps generate 6-digit rotating codes that refresh every 30–60 seconds.

***

## enable 2fa

## **what does it mean to “enable 2fa” for the company?**

enabling 2fa simply **turns on the feature** for your company. this means employees **can choose** to set up 2fa, but they are **not required** to do so. employees may set it up voluntarily inside their portal.

key points:

* employees decide on their own if they want to activate 2fa
* 2fa becomes available in each employee’s profile
* employees who enable 2fa can also disable it anytime
* no login restrictions are applied

think of enabling as _allowing_ or _making 2fa available_.

## what are the main pages to manage your company's 2fa?

* **Security Settings** — use this page to turn employee 2fa on or off for the company and manage **Admin 2FA Enforcement**.
* **Employee 2fa Status** — use this page to review which employees have 2fa enabled and reset 2fa for an employee who cannot recover access on their own.

## before you begin: key 2fa terms

* **two-factor authentication feature** — makes 2FA available in the employee portal.
* **admin 2fa enforcement** — makes 2FA mandatory for **All Admins** or **Selected Admins**.
* **2fa status** — shows whether an employee already has 2FA enabled.
* **recovery codes** — one-time backup codes employees can use if they lose access to their authenticator app.
* **reset 2fa** — clears the employee's current 2FA setup so they must set it up again on their next login.

## security settings

use this page when you want to control whether employees can use 2fa and whether they are required to use it.

**navigation:** **Settings** → **Workforce** → **Security**

the page has two main sections:

* **Two-Factor Authentication Feature** — the company-level availability switch
* **Admin 2FA Enforcement** — the mandatory-use section for admins

the page also shows these actions:

* **view employee 2fa status**
* **edit**
* **save changes**
* **cancel**

## what does enabling 2FA mean for the company?

turning on **two-factor authentication feature** makes 2fa available to employees in their portal.

when the feature is on:

* employees can choose to set up 2fa
* employees who already use 2fa continue to log in with it
* no admin is required to use 2fa unless **Admin 2FA Enforcement** is also turned on

when the feature is off:

* employees cannot newly set up 2fa
* employee login challenges are bypassed
* admin 2FA Enforcement is turned off

## how do i enable 2fa for employees?

1. open **security settings**.
2. click **edit**.
3. turn **two-factor authentication feature** on.
4. click **save changes**.

## what happens after i enable the feature?

employees can set up 2fa in their employee portal. Setting up 2fa is still optional unless you also turn on **Admin 2FA Enforcement** for admins. once 2fa is enabled for your company, employees will have the ability to set up 2FA on their ashima employee portal - [manage employee 2FA](../../../employee/portal/account-and-orientation/set-up-and-use-two-factor-authentication.md)

***

## enforcing 2fa

## what does admin 2fa enforcement mean?

use **Admin 2FA Enforcement** when 2fa should be required for **All Admins** or **Selected Admins**. Employee enforcement is configured separately and can apply to **All Employees**, **Selected Employees**, **Selected Departments**, or **Selected Payroll Groups**.

## how do i enforce 2fa?

1. open **Security Settings**.
2. click **edit**.
3. make sure **two-factor authentication feature** is on.
4. turn **Admin 2FA Enforcement** on.
5. choose **All Admins** or **Selected Admins**.
6. if needed, select the admins to include.
7. click **save changes**.

## fields

* **two-factor authentication feature** — turns employee 2fa availability on or off for the company.
* **admin 2fa enforcement** — makes 2fa mandatory for the selected admin scope.
* **all admins** — requires every admin to use 2fa.
* **selected admins** — requires only selected admins to use 2fa.

## distinguish administrator and employee enforcement

for administrators, enforcing 2fa means 2fa is required for **All Admins** or **Selected Admins**. Employee enforcement remains a separate setting with its own employee, department, and payroll-group scopes.

## what happens after enforcement is turned on?

review the saved Admin 2FA Enforcement selection in **Security Settings**.

## can i turn off enforcement later?

yes. you can turn off **Admin 2FA Enforcement** at any time.

1. open **Security Settings**.
2. click **edit**.
3. Turn **Admin 2FA Enforcement** off.
4. click **save changes**.

## what happens after enforcement is turned off?

review the saved Admin 2FA Enforcement selection in **Security Settings**.

***

## employee 2fa status

use this page to review employee 2fa completion and support employees who can no longer recover access on their own.

**navigation:** **Settings** → **Workforce** → **Security** → **view employee 2fa status**

the page shows a table with:

* **Name**
* **Employee ID**
* **Department**
* **Payroll Group**
* **2fa Status**
* **Action**

the **2fa Status** column shows:

* **enabled** — the employee already has 2fa enabled
* **not set** — the employee has not enabled 2fa

## how do i filter or search this page?

you can narrow the list using:

* **search employees**
* **status**
* **department**
* **payroll group**

***

## reset an employee's 2FA

## when should i reset an employee's 2fa?

use **reset 2fa** only when the employee cannot recover access using normal self-service options.

typical examples:

* the employee no longer has access to their authenticator app
* the employee no longer has their recovery codes
* the employee cannot complete login and cannot recover access on their own

{% hint style="info" %}
**note:** do not use reset as the first step if the employee can still log in with recovery codes or can still manage their own 2FA setup.
{% endhint %}

## how do i reset an employee's 2fa?

1. open **employee 2fa status**.
2. find the employee.
3. click **reset 2fa**.
4. review the confirmation message.
5. click **confirm reset**.

## what happens after i reset 2fa?

the reset clears the employee's current 2fa secret and recovery codes. the employee is prompted to set up 2fa again on their next login.

## rules and warnings

* Reset 2fa only affects the selected employee.
* Reset 2fa removes the employee's existing 2fa setup.
* after reset, the employee must complete setup again before 2fa can be used on the account.

## what should administrators know about employee self-service recovery?

employees are expected to manage normal 2FA recovery through their own portal whenever possible.

that includes:

* entering a valid authenticator code
* using a recovery code during login
* regenerating recovery codes while they still have account access

admin reset is the fallback when self-service recovery is no longer possible.

***

## continue in the affected module

* [manage employee 2FA](../../../employee/portal/account-and-orientation/set-up-and-use-two-factor-authentication.md)
