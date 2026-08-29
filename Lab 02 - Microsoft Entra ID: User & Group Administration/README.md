## Lab 02 - Microsoft Entra ID: User & Group Administration

## Objectives
- Manage Microsoft Entra ID user identities and verify employee account information.
- Create department-based security groups for HR, Finance, and IT.
- Manage security group memberships by adding and removing users based on department.
- Simulate an employee department transfer by moving a user between security groups.

## Scenario
We are administering identities for a small company. HR, Finance, and IT employees need to be organized into groups so access can be managed based on their departments.

We'll use the users from Lab 1:
Sarah Johnson — HR
David Miller — Finance
Michael Brown — IT

## Steps 
1. Now we would Open Microsoft Entra Admin Center by Going  to the Microsoft Entra admin center at entra.microsoft.com and Sign in using your Microsoft 365 administrator account.
<img width="2728" height="1702" alt="1" src="https://github.com/user-attachments/assets/b0a706b0-0f52-40b0-9058-3032a98eec40" />

2. On the left, select Identity.
   Select Users → All users.
<img width="2734" height="1722" alt="2" src="https://github.com/user-attachments/assets/c68b9eb1-1d41-499f-88c7-8ebfb259d7fd" />

3.  Now lets verify our user Sarah Johnson.
Click Sarah Johnson.
Open Properties.
Verify her:
Display name
User principal name
Job title
Account status
<img width="2736" height="1692" alt="3" src="https://github.com/user-attachments/assets/1e5e74db-db27-46c6-9cb5-1ae4e13b76bc" />

4.  Now lets create a security group.
   Click Groups on the left.
   Click All groups.
<img width="2736" height="1728" alt="4" src="https://github.com/user-attachments/assets/117b02d1-fd96-41d3-8094-58f6a9e39689" />

5. At the top, click New group.
<img width="2736" height="1618" alt="5" src="https://github.com/user-attachments/assets/2e14996d-f15c-467c-ac46-a66e331ec2e9" />

6.  Set Group type → Security.
For our lab, we'd use:
Group name: HR-Security
Group description: Provides HR employees access to HR resources
Membership type: Assigned
Then click on create.
<img width="2734" height="1800" alt="6" src="https://github.com/user-attachments/assets/e6dce403-6b0b-410f-8a02-8991626ed18e" />

7. Confirmation of our HR Security group creation
<img width="2736" height="1642" alt="7" src="https://github.com/user-attachments/assets/729b5fa2-2451-471c-9f3e-53b202bcf853" />

8.  Now lets Add Sarah to the HR Group
   Open HR-Security.
   Select Members.
   Click Add members.
<img width="2736" height="1722" alt="8" src="https://github.com/user-attachments/assets/d969f254-0a85-4bf9-a997-a00d478ffed9" />

9.  Search for Sarah Johnson.
   Select Sarah.
   Click Select
<img width="2720" height="1646" alt="9" src="https://github.com/user-attachments/assets/49e1d38b-877c-45fc-9194-8e37ec86ecf1" />

10. Confirmation of Sarah as a member of HR Security
<img width="2736" height="1644" alt="10" src="https://github.com/user-attachments/assets/6a919d7d-ca2d-4de9-86c6-e7f7c8cdc76d" />

11. Now we would also Create Finance and IT Groups
Repeat the process.
Security Group	Member
HR-Security	Sarah Johnson
Finance-Security David Miller
IT-Security	Michael Brown

<img width="2736" height="1636" alt="11" src="https://github.com/user-attachments/assets/515ff980-db0c-4446-9f1a-3bf1891400a4" />

12.  Lets Remove and Re-add a User from one department to another department
Let's simulate an employee changing departments.
Open Finance-Security.
Go to Members.
Select David Miller.
Click Remove.
Confirm.
<img width="2736" height="1674" alt="12" src="https://github.com/user-attachments/assets/6aa7aa5b-d6a0-45dc-98a3-999a323e95d5" />

13. Then we go to HR-Security , click on Members and click on Add members
<img width="2732" height="1640" alt="13" src="https://github.com/user-attachments/assets/7c6f9710-32f9-4d81-a185-d28c706e0d62" />

14. Select the miler and click on select
<img width="2736" height="1620" alt="14" src="https://github.com/user-attachments/assets/4c042ac8-4622-4377-9cad-fb4dbbf2b351" />

15. Confirmation  of David Miller in a new security group.
<img width="2736" height="1718" alt="15" src="https://github.com/user-attachments/assets/4331bda8-08ec-4243-90d8-52523b32928b" />


















