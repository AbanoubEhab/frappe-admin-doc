---
title: Sales Invoice
draft: true
tags:
  - Doctype
---
# Doctype: Sales Invoice
## **Fields:**
https://docs.google.com/spreadsheets/d/1kBmmoSOkUqpqTbHccBxBFrdUUDygoFPyATJZ_i12New/edit?usp=sharing
## **Validations:**

## **Workflow:**

![[Invoice.png]]

## **Permissions:**
- Read: R
- Write: W
- Create: C
- Delete: D

| Role             | Level 0 | Level 1 |
| ---------------- | ------- | ------- |
| Invoice Creator  | R/W/C   | R/W     |
| Invoice Approver | R/W     | R       |
| Finance Manager  | R/W     | R/W     |
| Sales Manager    | R/W     | R       |
| Legal Manager    | R/W     | R       |
| Revenue Officer  | R/W/C   | R/W     |
| Frappe Lord      | R/W/C/D | R/W     |
| System Manager   | R/W/C/D | -       |
## View Filters:

## Special Scripts:  

- When Apply VAT Checkbox in breakdown tab checked a code will calculate the VAT automatically
-  When Apply Withholding Tax Checkbox in breakdown tab checked a code will calculate the Apply Withholding Tax automatically
## Child tables:

### Contacts
![[Contacts]]

### Expanse Breakdowns

![[Expense Breakdowns]]



