---
title: General Cash PC
draft: false
tags:
  - Doctype
---
# Doctype: General Cash PC
## **Fields:**
https://docs.google.com/spreadsheets/d/1w7vY3UZ3S9hHlbo8vrSMQMKayrErjYRe4uw1XU4KjQ4/edit?usp=sharing
## **Validations:**

## **Workflow:**

![[Pasted_image_20250212125946.png]]

## **Permissions:**
- Read: R
- Write: W
- Create: C
- Delete: D

| Role              | Level 0 | Level 1 |
| ----------------- | ------- | ------- |
| PC Cash Requestor | R/W/C/D | R/W     |
| PC Cash Acceptor  | R/W     | R       |
| PC Cash Reviewer  | R/W     | R       |
| Finance           | R/W     | R       |
| Frappe Lord       | R/W/C/D | R/W     |
| System Manager    | R/W/C/D | -       |
## View Filters

Finance : Can see all Request bypassing any other restrictions
PC Cash Requestor : Can see only his requests
PC Cash Acceptor : Can see requests that is he assigned as Acceptor in the PC Cash asset that is linked to the request
PC Cash Reviewer : Can see requests that is he assigned as Reviewer in the PC Cash asset that is linked to the request
## Special Scripts:  

When Project PC is Approved A Payment Request will be created automatically and The Project PC will be moved automatically to Pending Closure
## Child tables:

![[Petty Cash Descriptions]]