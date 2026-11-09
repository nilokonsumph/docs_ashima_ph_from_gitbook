# configure account password and lock policies

set password and login-attempt policies for the subscription account, and review reset limits before requesting a reset.

**navigation:** owner/designated administrator's **Control Center → Security**

## review the account-wide impact

> **important:** these settings apply across the subscription account, not just the selected company. relevant reset-date changes can affect accounts across that subscription. check the intended account before confirming.

two-factor authentication is a separate control; see the existing [2FA guide](../../workforce/portal-time-and-security-access/manage-employee-and-administrator-2fa.md).

## configure the policy

1. choose **Edit**.
2. review password length and reuse, optional special-character and mixed-case requirements, and login-attempt and block-duration fields. alphabet and numeric requirements are fixed on.
3. choose the rotation setting: **Never**, **Every 30 days**, or **Custom**. supply the days for a custom interval.
4. choose **Update**, complete the confirmation, and check saved feedback. use **Cancel** to return to saved settings without keeping draft changes.

the page accepts a password length from **4 to 128** characters and failed-login attempts from **0 to 50**. a block duration uses **minute**, **hour**, or **day**, with a value from **0 to 365**. a custom password-rotation interval must be numeric.

if failed-login attempts are configured, complete the block-duration fields. if a block-duration unit is selected, provide its value. alphabet and numeric requirements remain enabled; special-character and mixed-case requirements are optional account settings.

these ranges describe what the page accepts. they are not a recommendation for the company’s security policy.

## request a reset separately

use the separate **Edit Reset** / **Reset** confirmation flow when a reset is intended. check its confirmation and result separately from saving policy settings.

**if rotation is set to Never:** a reset does not force a password change at the next sign-in. choose a rotation interval when periodic password changes are required.

## related articles

* [two-factor authentication (2FA)](../../workforce/portal-time-and-security-access/manage-employee-and-administrator-2fa.md)

***
