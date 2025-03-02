---
title: Payment Request
draft: false
tags:
  - Doctype
---
# Doctype: Payment Request
## **Fields:**
https://docs.google.com/spreadsheets/d/1MVAfaseFVzGLnn7N5io5YbbdJUXydmNSw3A7Y8_0W8U/edit?usp=sharing
## **Validations:**

- when a Payment request state = Pending Acceptor confirmation or Pending Project Manager Confirmation , the Acceptor cannot send the review Unless he selects the Payments term(s) he wants to send , And Actions Button will be hidden


## **Workflow:**

![[Pasted_image_20250216142207.png]]

## **Permissions:**
Read: R
Write: W
Create: C
Delete: D

|                             | Level 0 | Level 1 | Level 2 | Level 3 |
| --------------------------- | ------- | ------- | ------- | ------- |
| System Manager              | R/W/C/D | R/W     | R/W     | -       |
| Administration              | R/W     | R/W     | R       | -       |
| PO Requestor                | R       | R       | R       | -       |
| WO Requestor                | R       | R       | R       | -       |
| Urgent Requestor            | R       | R       | -       | -       |
| Project PC Requestor        | R       | R       | -       | -       |
| Urgent Project PC Requestor | R       | R       | R       | -       |
| PC Cash Requestor           | R       | R       | R       | -       |
| PC Credit Requestor         | R       | R       | R       | -       |
| PC Credit Acceptor          | R/W     | -       | R       | -       |
| PC Credit Special Acceptor  | R/W     | -       | R       | -       |
| PC Cash Acceptor            | R/W     | R       | -       | -       |
| PC Cash Reviewer            | R       | R       | -       | -       |
| PC Credit Reviewer          | R       | R       | R       | -       |
| PO Acceptor                 | R/W     | R       | R/W     | -       |
| WO Acceptor                 | R/W     | R       | R/W     | -       |
| PO Reviewer                 | R       | R       | R       | -       |
| WO Reviewer                 | R       | R       | R       | -       |
| PO Approver                 | R       | R       | R       | -       |
| WO Approver                 | R       | R       | R       | -       |
| Urgent Approver             | R       | R       | R       | -       |
| PO Archivist                | R       | R       | R       | -       |
| WO Archivist                | R       | R       | R       | -       |
| Project Manager             | R/W     | R       | R/W     | -       |
| Finance                     | R       | R       | R       | R       |
| Finance Manager             | R       | R       | -       | R/W     |
| Frappe Lord                 | R/W/C/D | R/W     | R/W     | R/W     |
| Payment Run Reviewer        | R       | -       | -       | -       |
| Payment Run Approver        | R       | -       | -       | -       |
| Payment Run Transferrer     | R       | -       | -       | -       |


## View Filters

* *Note: The original Requestor of the Source request Becomes the owner of the Payment request

- Finance : Can see all Request bypassing any other restrictions
- Administration : If the payment request Created from (PO/WO/Urgent PO/Urgent WO)
- PC Cash Acceptor/PC Credit Acceptor/PC Credit Special Acceptor : Can see if he is the Acceptor of the Original Request
- PO/WO Acceptor : Can see his department Requests and the source request is (PO/WO/Urgent PO/Urgent WO)
- Project Manager : can see his project Request and the Source request is (PO/WO/Urgent PO/Urgent WO)
- PO Archivist :  If the payment request Created from (PO/Urgent PO)
- WO Archivist : If the payment request Created from (WO/Urgent WO)
- Urgent Requestor : Can see his requests


## Special Scripts:  

- The payment Request is being created automatically by (PO - WO - EO - General Cash PC - General Credit Card PC - Project PC - Urgent Project PC - Urgent PO - Urgent WO ) when any of them Approved
- A Script will check for Request source to send the request to the appropriate state which is shown in the Workflow  
- When all Payment Terms in the request checked as Submitted , the request state changes to pending Review
- When all Payment Terms in the request checked as Reviewed , the request state changes to pending Approval
- When all Payment Terms in the request checked as Approved , the request state changes to pending Transfer
- When all Payment Terms in the request checked as Transferred , the request state changes to Completed

## Child tables:

### Payment Term:
![Payment_Term_(Payment_Request)](Payment_Term_(Payment_Request).md)


# Other Notes

- when Transferrer Complete the request He chose from Complete Through Bank and Complete Through PC which checks the checkbox's in the Payments Terms
-  In The states Pending Review, Pending Approval and Pending Transfer the User interact with the request Using the Reports (the users that have authority to change in payment request can change directly without reports)

- the Checkboxes (Submitted , Reviewed ,Transferred, bank ,PC ) in Payment Term Child table changes automatically when the User selects the Payment Term and take action on it