# assign and print Workforce documents

Use Workforce documents to prepare a document request for an employee, check its approval status and print the approved output.

**Navigation:** **Utilities → Documents**.

## create the employee’s document request

1. Search the document list and open the employee’s list, or start from the main list. Select **Create document**.
2. Check the employee already selected, or select the intended employee if none is preselected.
3. Choose the exact **Document Name** and check its read-only **Document Type**. Before saving, review the employee and certificate you intend to issue.
4. Select **Save** to submit the request. Correct selection errors before trying again. **Cancel** closes the form without saving.
5. Check the request and approval status in the refreshed list.

An active published **Business Content** certificate can be selected by its document name without a separate content assignment. It uses the current published version when the request is saved. Other Document Manager certificates can have different output behavior, as explained below.

## check the saved content before printing

Open the request and review its document name, type, request date, approval information and body. **Print Preview** is available for approved output; a newly created request is not automatically ready to print.

| document source              | what happens when information changes later                                                                                                                                                                                                                                                                              |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Business Content certificate | Saving retains the selected version, title, body and employee/request details. Later template publication or employee-profile changes do not rebuild that saved request. Final approval adds the actual signatory using the saved details.                                                                               |
| Document Manager certificate | Utilities can use the current certificate body and employee details. Employee and To Do views use stored request content when present, otherwise the certificate body, with employee substitutions. Check the actual output where you intend to use it; these views are not a guarantee of an unchanged historical copy. |

If employee details are wrong, correct the owning employee record. Then review the document again. That correction alone does not update an existing Business Content request’s saved content.

## print the approved document

1. Open the approved request and select **Print Preview**.
2. Check the employee, document body and signatory before printing.
3. Select **Print** and follow the displayed **Letter**, **Portrait**, **Shrink to Fit** and blank browser headers/footers guidance.

## correct or remove a request

A saved request has no supported update editor. Check the document source and saved content before replacing it. To remove a request, select only the intended row, choose **Delete**, confirm, and verify the refreshed list.

{% hint style="warning" %}
Removing a request cannot retrieve copies already printed or shared. Review those copies before issuing a replacement.
{% endhint %}

## why is a document or employee missing?

Check your page permission, employee visibility, confidential access, employee status and whether the document is available for the company. For a request awaiting a decision, use the configured [Document Workflow and To Do](../todo-workflow/request-specific-approvals/review-document-requests.md). Approval and external delivery are separate outcomes.
