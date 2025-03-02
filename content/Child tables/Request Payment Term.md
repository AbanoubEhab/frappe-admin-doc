
| Label               | Name                | **Type** | **Prem Level** | **Mandatory** | **Hidden** | **Read Only** | Set Only once | Display Depends On (JS)               | Mandatory Depends On (JS)             |
| ------------------- | ------------------- | -------- | -------------- | ------------- | ---------- | ------------- | ------------- | ------------------------------------- | ------------------------------------- |
| Installment Date    | installment_date    | Date     | 0              | Yes           | No         | No            | No            |                                       |                                       |
| Percentage of Total | percentage_of_total | Percent  | 0              | No            | Yes        | No            | No            |                                       |                                       |
| Installment Amount  | installment_amount  | Currency | 0              | Yes           | No         | No            | No            |                                       |                                       |
| Vendor              | vendor              | Link     | 0              | No            | No         | Yes           | No            | eval:parent.party_type == 'Vendor'    | eval:parent.party_type == 'Vendor'    |
| freelancer          | freelancer          | Link     | 0              | No            | No         | No            | No            | eval:parent.party_type == 'Freelance' | eval:parent.party_type == 'Freelance' |
| operative_details   | operative_details   | Attach   | 0              | No            | No         | No            | No            | eval:parent.party_type == 'Operative' | eval:parent.party_type == 'Operative' |
