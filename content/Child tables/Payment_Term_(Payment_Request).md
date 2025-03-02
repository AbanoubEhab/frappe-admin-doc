
| Label                | Name                 | Non Negative | **Type**  | **Prem Level** | **Mandatory** | **Hidden** | **Read Only** | Display Depends On (JS)               | Mandatory Depends On (JS)             |
| -------------------- | -------------------- | ------------ | --------- | -------------- | ------------- | ---------- | ------------- | ------------------------------------- | ------------------------------------- |
| Installment Date     | installment_date     | -            | Date      | 2              | Yes           | No         | No            | -                                     | -                                     |
| Percentage of Total  | percentage_of_total  | -            | Percent   | 0              | No            | Yes        | No            | -                                     | -                                     |
| Installment Amount   | installment_amount   | -            | Currency  | 2              | Yes           | No         | No            | -                                     | -                                     |
| Vendor               | vendor               | -            | Link      | 0              | No            | No         | Yes           | eval:parent.party_type == 'Vendor'    | -                                     |
| freelancer           | freelancer           | -            | Link      | 0              | No            | No         | Yes           | eval:parent.party_type == 'Freelance' | -                                     |
| Freelancer Agreement | Freelancer_agreement | -            | Attach    | 1              | No            | No         | No            | eval:parent.party_type == 'Freelance' | eval:parent.party_type == 'Freelance' |
| operative_details    | operative_details    | -            | Attach    | 1              | No            | No         | No            | eval:parent.party_type == 'Operative' | eval:parent.party_type == 'Operative' |
| Payment Group        | payment_group        | Yes          | Int       | 0              | No            | No         | Yes           | -                                     | -                                     |
| Submitted            | submitted            | -            | Check     | 0              | No            | No         | Yes           | -                                     | -                                     |
| Reviewed             | reviewed             | -            | Check     | 0              | No            | No         | Yes           | -                                     | -                                     |
| Approved             | approved             | -            | Check     | 0              | No            | No         | Yes           | -                                     | -                                     |
| Transferred          | transferred          | -            | Check<br> | 0              | No            | No         | Yes           | -                                     | -                                     |
| Bank                 | bank                 | -            | Check<br> | 3              | No            | No         | No            | -                                     | -                                     |
| PC                   | pc                   | -            | Check     | 3              | No            | No         | No            | -                                     | -                                     |


