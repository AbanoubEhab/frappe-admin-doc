
| Label       | Name        | **Type**   | **Options** | **Prem Level** | **Mandatory** | **Read Only** | Display Depends On (JS)     | Mandatory Depends On (JS)   |
| ----------- | ----------- | ---------- | ----------- | -------------- | ------------- | ------------- | --------------------------- | --------------------------- |
| Description | description | Small Text | -           | 0              | Yes           | No            | -                           | -                           |
| Item        | item        | Data       | -           | 0              | No            | No            | eval:doc.parenttype == 'PO' | eval:doc.parenttype == 'PO' |
| Quantity    | quantity    | Int        | -           | 0              | Yes           | No            | -                           | -                           |
| Unit Price  | unit_price  | Currency   | Currency    | 0              | Yes           | No            | -                           | -                           |
| Total       | total       | Currency   | Currency    | 0              | Yes           | Yes           | -                           | -                           |