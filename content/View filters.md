# PO

- PO requestor : Can see only his POs
- PO Acceptor : Can see His department(s) POs in any state except for state = Draft
- Project Manager : Can see POs that he is the project Manager of it and NOT in the states (Draft/Pending Amendment/Pending Acceptance/Acceptor On-Hold/Rejected by Acceptor)
- PO Reviewer : Pending Reviewal / Reviewer On-Hold / Pending Approval / Approver On-Hold 
- PO Approver / Finance Manager : Pending Approval / Approver On-Hold / Approved / Rejected by Approver
- PO Archivist / finance : Approved

# EO

- Legal : Can see the requests he Created only
- Finance Manager : Can see all requests that is not draft
- Finance : Can see the requests he created or the requests in state = Approved

# Urgent PO/WO

- Urgent Requestor : Can see only the requests he Created only
- Urgent Approver : Can see only the requests he was set as acceptor

# Project PC

- Project PC Requestor : Can see only the requests he created
- Project Manager : Can see only the requests linked to his projects

# Urgent Project PC

- Urgent Project PC Requestor : Can see only the requests he created
- Project Manager : Can see only the requests linked to his projects

# General Cash PC

Finance : Can see all Request bypassing any other restrictions
PC Cash Requestor : Can see only his requests
PC Cash Acceptor : Can see requests that is he assigned as Acceptor in the PC Cash asset that is linked to the request
PC Cash Reviewer : Can see requests that is he assigned as Reviewer in the PC Cash asset that is linked to the request

# General Credit PC

- Finance : Can see all Request bypassing any other restrictions
- PC Credit Requestor : Can see only his requests
- PC Credit Acceptor : Can see requests that is he assigned as Acceptor in the PC Credit Card asset that is linked to the request
- PC Credit Reviewer : Can see requests that is he assigned as Reviewer in the PC Credit Card that is linked to the request

# Payment Request

- Finance : Can see all Request bypassing any other restrictions
- Administration : If the payment request Created from (PO/WO/Urgent PO/Urgent WO)
- PC Cash Acceptor/PC Credit Acceptor/PC Credit Special Acceptor : Can see if he is the Acceptor of the Original Request
- PO/WO Acceptor : Can see his department Requests and the source request is (PO/WO/Urgent PO/Urgent WO)
- Project Manager : can see his project Request and the Source request is (PO/WO/Urgent PO/Urgent WO)
- PO Archivist :  If the payment request Created from (PO/Urgent PO)
- WO Archivist : If the payment request Created from (WO/Urgent WO)
- Urgent Requestor : Can see his requests