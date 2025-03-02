---
title: Urgent PO
draft: false
tags:
  - Doctype
---
# Doctype: Urgent PO
## **Fields:**
https://docs.google.com/spreadsheets/d/17tTDwYGQhtA-uiB5IQIA-oqsokfmrDkgcfR5ZsYErRI/edit?usp=sharing
## **Validations:**

- On Saving a code will Compare Total of Payment Terms to Total Field and if they not Equal it will prevent the user from saving 
- On Saving a code will check if Using a date in the Past in Payment Terms and will prevent the user from saving 
## **Workflow:**

![[Pasted_image_20250210150515.png]]
## **Permissions:**
Read: R
Write: W
Create: C
Delete: D

|                  | Level 0 | Level 1 | Level 2 |
| ---------------- | ------- | ------- | ------- |
| Urgent Requestor | R/W/C   | R/W     | -       |
| Urgent Approver  | R/W     | R       | R       |
| PO Archivist     | R       | R       | R       |
| Finance          | R       | R       | -       |
| Finance Manager  | R       | -       | R       |
| Frappe Lord      | R/W/C/D | R/W/D   | R/W/D   |
| System Manager   | R/W/C/D | R       | R/W/D   |
## View Filters

Urgent Requestor : Can see only the requests he Created only
Urgent Approver : Can see only the requests he was set as acceptor

## Special Scripts:  

When A PO is completed a Script will create A new Payment Request Using the data from The PO and will link the New Payment request to Payment Request Field

## Child tables:

### Request Descriptions:

![[Request Descriptions]]

### Additional Fees:

![[Request Additional Fees]]

### Payment Term:
![[Request Payment Term]]



