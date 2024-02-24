### Example Access Contorls worksheet 

# Scenario 
Recently, a deposit was made from the business to an unknown bank account. The finance manager says they didn’t make a mistake. Fortunately, they were able to stop the payment. The owner has asked you to investigate what happened to prevent any future incidents.

To do this, you’ll need to do some accounting on the incident to better understand what happened. First, you will review the access log of the incident. Next, you will take notes that can help you identify a possible threat actor. Then, you will spot issues with the access controls that were exploited by the user. Finally, you will recommend mitigations that can improve the business' access controls and reduce the likelihood that this incident reoccurs.

|--------------------------- |    Notes                                                |     Issue                                       | Recommendations |
|------------------------------|---------------------------------------------------------|-------------------------------------------------|-----------------|
|Authorization/authentication  | Time of access 10/03/2023, at 8:29 AM  by Leagal/Administrator, IP address : 152.207.255 255              |   Robert Taylor Jr is an admin. His contract ended in 2019, but his account accessed payroll systems in 2023.          |   User accounts should expire after 30 days. Contractors should have limited access to business resources.  Enable MFA.              | 