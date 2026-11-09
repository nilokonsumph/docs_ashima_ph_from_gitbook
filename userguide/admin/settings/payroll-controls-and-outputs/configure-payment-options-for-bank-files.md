# configure payment options for bank files

use **Payment Options** to save the company identifiers and bank-specific fields required by Ashima's supported bank-file formats. A saved option prepares the format configuration; it does not send money or confirm that a bank accepted a generated file.

**navigation:** go to **Settings → Paycheck → Payment Options**.

## choose a supported bank

at the inspected source version, the add form offers **Rizal Commercial Bank Corporation**, **Metrobank**, **Banco de Oro**, **Union Bank**, **BPI**, and **Security Bank**. a bank already configured for the company is removed from the add list, so the company normally maintains one active option per bank format.

## enter the fields for the selected format

the form changes with the selected bank. depending on the format, it can request:

* **Company Code**;
* **Organizational Short Code**;
* **Company Account Number**;
* **Depository Branch Code**;
* **Funding Account**;
* **Payroll Branch Code**;
* BDO upload date and batch;
* HDMF-payment enablement and branch code; and
* BPI **ExpressLink** or **BizLink** enablement.

**Union Bank** requires **Organizational Short Code**. most formats other than **Union Bank** and **Security Bank** require **Company Code** in the current create path. other fields are saved only for the bank or optional service that uses them.

## add and verify a payment option

1. select the add action.
2. choose the bank.
3. complete the fields displayed for that format using identifiers confirmed with the bank.
4. enable HDMF payment, **ExpressLink**, or **BizLink** only when the company uses that supported service, then complete the dependent fields.
5. save and open the bank detail page.
6. compare the saved identifiers with the bank's approved setup.
7. generate a test output through the applicable payroll or disbursement workflow and validate it through the company's normal bank-file control process.

{% hint style="warning" %}
**warning:** a successful save proves only that Ashima stored the configuration. it does not validate the identifiers with the bank, transmit a payment, or guarantee file acceptance.
{% endhint %}

\## continue in the affected module

* [review payroll payment outputs](../../paycheck/)
