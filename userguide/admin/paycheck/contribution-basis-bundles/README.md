# contribution basis bundles

{% hint style="info" %}
**Availability:** Contribution basis is being prepared for release. Continue using your current **Contribution Rules** for now. The steps below apply after your company is given access and bundle-based payroll calculation is enabled.
{% endhint %}

A contribution basis bundle lets your company choose which payroll-recognized earnings and adjustments form the basis for SSS, PhilHealth, or Pag-IBIG. The contribution method and table then use that basis to calculate the contribution.

The important new choice is **who uses each basis**. Instead of relying on one general contribution rule for everyone, you can create more than one bundle for a contribution, set a company default, and assign a different saved bundle to one employee or to several selected employees. For example, you can filter the employee list by **Payroll group** and assign a bundle to everyone you select from that group. This is a bulk assignment to those employees, not an automatic rule for everyone who joins the group later.

| setup                                                | who uses it                                                                                                                                                                              |
| ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Company default** for SSS, PhilHealth, or Pag-IBIG | Employees without a separate bundle assignment for that contribution.                                                                                                                    |
| **Employee assignment**                              | One selected employee, or several employees selected together using filters such as **Payroll group**. Their saved assignment takes precedence over that contribution's company default. |

Creating a bundle only saves the available basis. To use it, save it as the company default or assign it to selected employees. [Configure contribution basis bundles](configure-contribution-basis-bundles.md) explains both steps.

When this feature is enabled for your company, open **Settings → Paycheck → Contribution basis** to review or change the setup. For the separate rules that determine contribution timing and calculation, see [configure contribution timing and calculation rules](../pay-items-contributions-and-tax/configure-contribution-timing-and-calculation-rules.md).

Choose the guide that matches your company:

| your situation                                                                            | start with                                                                                                                                                                                                          |
| ----------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| You already have SSS, PhilHealth, or Pag-IBIG contribution rules with **Yes** selections. | [Review and migrate existing contribution rules](migrate-existing-contribution-rules.md) before setting up a new bundle. The review shows what will become each company's default and what will remain unchanged.   |
| You are setting up a new basis, or migration is already complete.                         | [Configure contribution basis bundles](configure-contribution-basis-bundles.md) to create a bundle, set the company default, and assign a different bundle to an individual or selected members of a payroll group. |

For example, an existing SSS rule might include **Basic pay**, **Overtime pay**, and **Night shift differential**. Migration can copy those **Yes** selections into an SSS bundle and make it the SSS company default. The review also shows PhilHealth and Pag-IBIG, so check all three before confirming.

{% hint style="info" %}
Saving or importing a basis does not recalculate an existing pay run. Check an eligible open pay run only after your company has enabled bundle-based calculation. Existing payroll and contribution tables are separate from the bundle setup.
{% endhint %}
