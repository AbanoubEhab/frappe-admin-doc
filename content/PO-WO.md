---
title: PO-WO
draft: false
tags:
  - Doctype
---
# Doctype: PO 
## **Fields:**
https://docs.google.com/spreadsheets/d/1ebg2LNu-rrh0DMWXZs0dG6W2WPWUHgko8yLzvOsX5gs/edit?usp=sharing
## **Validations:**

- On Saving a code will Compare Total of Payment Terms to Total Field and if they not Equal it will prevent the user from saving 
- On Saving a code will check if Using a date in the Past in Payment Terms and will prevent the user from saving 
## **Workflow:**

### If General (allocation = General)

![[Pasted_image_20250203174147.png]]

### If Project (allocation = Project)

![[Pasted_image_20250203174308.png]]

## **Permissions:**
Read: R
Write: W
Create: C
Delete: D

|                 | Level 0 | Level 1 | Level 2 | Level 3 |
| --------------- | ------- | ------- | ------- | ------- |
| PO Requestor    | R/W/C   | R/W     | R       | -       |
| PO Acceptor     | R/W     | R       | R/W     | -       |
| Project Manager | R/W     | R       | R       | R       |
| PO Reviewer     | R/W     | R       | R       | -       |
| PO Approver     | R/W     | R       | R       | R       |
| PO Archivist    | R       | R       | R       | -       |
| Finance         | R       | R       | R       | -       |
| Finance Manager | R/W     | R       | R       | R       |
| Frappe Lord     | R/W/C/D | R       | R/D     | R/W/D   |
| System Manager  | R/W/C/D | R       | R/W     | R/W/D   |
## View Filters

- PO requestor : Can see only his POs
- PO Acceptor : Can see His department(s) POs in any state except for state = Draft
- Project Manager : Can see POs that he is the project Manager of it and NOT in the states (Draft/Pending Amendment/Pending Acceptance/Acceptor On-Hold/Rejected by Acceptor)
- PO Reviewer : Pending Reviewal / Reviewer On-Hold / Pending Approval / Approver On-Hold 
- PO Approver / Finance Manager : Pending Approval / Approver On-Hold / Approved / Rejected by Approver
- PO Archivist / finance : Approved
## Special Scripts:  

When A PO is completed a Script will create A new Payment Request Using the data from The PO and will link the New Payment request to Payment Request Field

## Child tables:

### Request Descriptions:

![[Request Descriptions]]

### Additional Fees:

![[Request Additional Fees]]

### Payment Term:
![[Request Payment Term]]



