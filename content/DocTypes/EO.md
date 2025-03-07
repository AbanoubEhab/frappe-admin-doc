---
title: EO
draft: false
tags:
  - Doctype
---
# Doctype: EO
## **Fields:**
https://docs.google.com/spreadsheets/d/1vD16Jmse9exJYzXhY-OBuspwzRbbc2Xr6SDBXmcMpU0/edit?usp=sharing
## **Validations:**

- On Saving a code will Compare Total of Payment Terms to Total Field and if they not Equal it will prevent the user from saving 
- On Saving a code will check if Using a date in the Past in Payment Terms and will prevent the user from saving 
## **Workflow:**

![[EO.png]]

## **Permissions:**
- Read: R
- Write: W
- Create: C
- Delete: D
- Submit: S

| Role           | Level 0 | Level 1 | Level 2 |
| -------------- | ------- | ------- | ------- |
| EO Requestor   | R/W/C   | R/W     | R       |
| EO Approver    | R/W     | R       | R/W     |
| Finance        | R       | R       | R       |
| System Manager | R/W/C/D | -       | -       |

## View Filters

Legal : Can see the requests he Created only
Finance Manager : Can see all requests that is not draft
Finance : Can see the requests he created or the requests in state = Approved

## Special Scripts:  

When an EO is completed a Script will create A new Payment Request Using the data from The EO and will link the New Payment request to Payment Request Field

## Child tables:

### Request Descriptions:

![[Request Descriptions]]


### Payment Term:

![[Request Payment Term]]



