## LAB 07 - Offboarding 

## Objectives 
- Secure departing employee accounts by blocking Microsoft 365 sign-in and resetting account credentials.
- Revoke organizational access by removing the employee from assigned security and Microsoft 365 groups.
- Manage license deprovisioning by removing the employee's Microsoft 365 license while retaining the account temporarily for data retention and handover.
- Verify successful access revocation by testing the former employee's previous credentials and confirming they can no longer access Microsoft 365 resources

## Steps 
1.  Before changing anything, lets go to:
Microsoft 365 Admin Center → Users → Active users → James Wilson
As we can see , he's account is active
<img width="2736" height="1640" alt="1" src="https://github.com/user-attachments/assets/2f70edbc-db3d-4ff1-ab30-7aa94f8a5d7d" />

2. Next we'd Block sign-in
Select: Block this user from signing in → Save
<img width="1298" height="1552" alt="2" src="https://github.com/user-attachments/assets/ade1f91a-3e66-4df6-a678-a9adc9f7a5be" />

3.  Next we'd click on reset password , and change it to a new password without giving the new one to james Wilson. Then we'd click on the reset password button to confirm this setting 
<img width="1304" height="1630" alt="3" src="https://github.com/user-attachments/assets/05585412-fc4c-4b8a-9400-dd99bc572bae" />

4. Next we'd click on manage groups and remove him from the existing groups 
<img width="1284" height="1650" alt="4" src="https://github.com/user-attachments/assets/62421170-eaba-4486-8ed5-0657d973168d" />

5. <img width="1328" height="1574" alt="5" src="https://github.com/user-attachments/assets/1cac38e1-7856-4960-b743-8115745742d6" />

6. Successfully removed him from the security groups
 James's mailbox/account was retained temporarily for organizational data-retention and handover requirements.
<img width="1302" height="1552" alt="6" src="https://github.com/user-attachments/assets/ccee1854-e374-4d66-8468-116738c10386" />

7. Here we would uncheck the box and click on save changes to make office 365 E3 subscription  not available to James Wilson
 <img width="1876" height="1620" alt="8" src="https://github.com/user-attachments/assets/6b272f09-fd1f-4eb6-bbe3-ced77a1cd370" />

8.  Now lets confirm if names can sign in with his old details
<img width="2730" height="1608" alt="9" src="https://github.com/user-attachments/assets/7e73f96d-a997-4b06-8e3a-ac135f12a49c" />
