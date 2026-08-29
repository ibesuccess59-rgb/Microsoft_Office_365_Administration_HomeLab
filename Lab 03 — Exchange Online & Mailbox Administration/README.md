## Lab 3 — Exchange Online & Mailbox Administration

## Objectives
By the end of this lab, we will:

- Manage user mailboxes
- Create an email alias
- Create a shared mailbox
- Assign shared-mailbox permissions
- Create a distribution list
- Test our Exchange configuration


## Scenario
We are the Microsoft 365 administrators for a small company. We need to manage employee mailboxes, create an email alias, configure a shared mailbox, create a distribution list, and assign mailbox permissions.


## Steps 

1. open admin.exchange.microsoft.com on our web browser
<img width="2732" height="1640" alt="1" src="https://github.com/user-attachments/assets/5a93aecf-6389-4164-94ac-0be9cbac97e2" />

2. Check Our User Mailboxes
   From the Exchange Admin Center: Go to Recipients, Click Mailboxes.
<img width="2736" height="1638" alt="2" src="https://github.com/user-attachments/assets/71eb8e33-2f97-415a-b1e6-bec9ae0d5760" />

3.  We should see the users from our previous labs:
   Sarah Johnson
   David Miller
   Michael Brown
<img width="2736" height="1658" alt="3" src="https://github.com/user-attachments/assets/a62e43a3-88be-4245-b164-bf4687cf3da0" />

4.  Click Sarah Johnson.
   Review her mailbox information.
   This proves: We can locate and administer Exchange Online user mailboxes.
<img width="2692" height="1658" alt="4" src="https://github.com/user-attachments/assets/5c03a8e4-77d2-44b1-8f18-5b7eddc39af7" />

5. Sarah's email address where she can be reached personally in the enterprise
<img width="1174" height="1698" alt="5" src="https://github.com/user-attachments/assets/3cf8e7de-3155-4f03-b8ec-06ff5fcab763" />

6. Now lets Create the shared mailbox , Click Add a shared mailbox for the IT department. A shared mailbox is basically a company email address that multiple employees can access and manage together, instead of belonging to one person.
<img width="2728" height="1638" alt="6" src="https://github.com/user-attachments/assets/360c370a-27b1-4364-9b19-e2d8f77cb818" />

7. Enter:
Display name: IT Support
Email address: itsupport@ibe146.onmicrosoft.com
Alias : IT Support then click on create.
<img width="1410" height="1670" alt="7" src="https://github.com/user-attachments/assets/8638fa7e-c408-4bc3-a48d-1e95063533f7" />

8. Confirmation of our shared ITSupport Inbox
<img width="1238" height="1658" alt="8" src="https://github.com/user-attachments/assets/8dfc9dd7-53fd-4127-92bf-322c663209c5" />

9. Now lets give Michael two permissions
   click on mailbox delegation
   We'd give Michael full access , under read and manage (full access)
   Click on edit
<img width="1448" height="1688" alt="9" src="https://github.com/user-attachments/assets/49a20a5c-512e-41c6-900d-0d7499925a94" />

10. In the mailbox delegation , click on add members
<img width="1396" height="1680" alt="10" src="https://github.com/user-attachments/assets/1b43925c-0e3c-4e48-b1e0-d6784568ecda" />

11. Select Michael Brown , then click on save , then click on confirm
<img width="1236" height="1678" alt="11" src="https://github.com/user-attachments/assets/49ed26b7-f6ce-4fa4-ade5-e3fdfdb7562c" />

12. Confirmation of Michael brown as a member of the IT-support shared inbox
<img width="2730" height="1632" alt="12" src="https://github.com/user-attachments/assets/5cfe73b6-b6f8-41be-b6b1-2a2de6fd8f8b" />

13. Here we would give Michael send as permission too in the IT-support mailbox, click on edit .
<img width="2730" height="1646" alt="13" src="https://github.com/user-attachments/assets/22de5981-af55-463f-a1dc-56cf95203561" />

14. click on add members , select Michael brown , click save . click confirm
<img width="1186" height="1710" alt="14" src="https://github.com/user-attachments/assets/52388b38-0e0f-4ba5-9e6f-2084d6c8b7f9" />

15. Confirmation of Michael Brown as a member in "Send as" permission
<img width="1180" height="1704" alt="15" src="https://github.com/user-attachments/assets/4330820d-4962-42e5-a4fc-a9fe9a052c4c" />

16. Now we create a distribution group.
    Recipients → Groups
    Click Add a group.
    Distribution list is simply ONE address that forwards/distributes an email to      multiple people's inboxes.
<img width="2726" height="1724" alt="16" src="https://github.com/user-attachments/assets/32fb7215-72bf-4655-9dc5-c1d5a3cd090f" />

17. For group type , choose distribution
<img width="2736" height="1650" alt="17" src="https://github.com/user-attachments/assets/1b251364-1ea6-4b6c-8cd5-a8617a097ad1" />

18. Enter:
Name: HR Department
Description: Distribution list for HR employees
Click Next.
<img width="1408" height="1698" alt="18" src="https://github.com/user-attachments/assets/48bc1fcf-42ae-46da-9d4d-5428cfac0ee8" />

19. Here we assign sarah as owner by clicking on assign owner , then select sarah , then we would click on next
<img width="1408" height="1694" alt="19" src="https://github.com/user-attachments/assets/df9a5018-d1f5-40ce-8c08-52c119a48c0d" />

20. Then we'll continue , next we create:
hrdepartment@ibe146.onmicrosoft.com
Set Joining the group to onwer's approval
And leave , allow people outside of my organization to send email to this distribution group unchecked.
<img width="1418" height="1696" alt="20" src="https://github.com/user-attachments/assets/0974e641-f550-465e-95a8-77a5a33ff0c9" />

21. Review our settings and click on create, which creates our distribution group.
<img width="1410" height="1746" alt="21" src="https://github.com/user-attachments/assets/b37739fe-50eb-4714-a685-1145881f4ac0" />

22. Confirmation of our HR distribution list created
<img width="2726" height="1680" alt="22" src="https://github.com/user-attachments/assets/110dec73-4b72-41d0-a058-9d3fb18e03f0" />

23.  Add Sarah to the Distribution List
Open : HR Department
Go to: Members
<img width="2726" height="1794" alt="23" src="https://github.com/user-attachments/assets/fb1d8a68-79cc-4789-94bb-81175156a3b9" />

24. search and select : Sarah Johnson
   click on add
   Now sarah johnson is an onwer and aslo a member
<img width="1174" height="1712" alt="24" src="https://github.com/user-attachments/assets/fbb36b3a-5ccd-47a9-bfb7-3a5aee2745f5" />

25. Confirmation of sarah johnson being onwer and memeber
<img width="1176" height="1714" alt="25" src="https://github.com/user-attachments/assets/364ff1b7-d17e-46a0-b9cc-717d0560191e" />
