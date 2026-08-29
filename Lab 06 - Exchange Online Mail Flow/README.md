## Lab 06 - Exchange Online Mail FLow

## Objectives 
- Create and configure Exchange Online mail flow rules to automate email handling based on specific senders and recipients.
- Implement automated HR email routing by configuring transport rules to automatically include designated HR personnel.
- Review Microsoft Defender anti-spam policies and understand how Exchange Online protects organizational email.
- Test and verify mail flow configurations using Outlook and Exchange Message Trace to confirm successful rule processing and email delivery.

## Scenario 
Microsoft 365 administrators responsible for corporate email security and mail flow. We need to configure a transport rule, review anti -spam controls, generate test email traffic, trace message delivery, and verify our configuration. 

## Steps 

1. Lets Open Exchange Admin Center

Sign in with our administrator account and open:
Exchange Admin Center
On the left, we should see areas such as:
Recipients
Mail flow
Reports
<img width="1306" height="1558" alt="1" src="https://github.com/user-attachments/assets/638d6269-f0c2-400e-9202-54c1605b7903" />

2. lets Create Our Mail Flow Rule
   On the left hand pane , click on rules , on the rules interface , click on add a rule , then confirm you want to create a new rule
<img width="1310" height="1634" alt="2" src="https://github.com/user-attachments/assets/e3d8637b-ffb7-4e06-bb69-4806987a91dd" />

3. This leads us to set rule conditions 
Enter:

Name: HR to James Priority Rule

IF
Sender = Sarah Johnson

AND

Recipient = James Wilson

THEN
Set Importance = High
<img width="2736" height="1650" alt="3" src="https://github.com/user-attachments/assets/dc484816-0699-42f4-9145-31db5dbf159d" />

4. Confirmation of rules
<img width="1326" height="1640" alt="4" src="https://github.com/user-attachments/assets/6463b1a9-2987-4acf-b898-dc0a9cdd50a8" />

5. Open: Microsoft Defender portal
Go to: Email & collaboration → Policies & rules
<img width="1342" height="1648" alt="5" src="https://github.com/user-attachments/assets/c5031621-1091-464f-96a8-8587066dc32e" />

6.  In the Policies and Rules Interface , We would click on Threat Policies
<img width="2728" height="1644" alt="6" src="https://github.com/user-attachments/assets/90a545fc-0d9b-402b-82c6-7db4db933888" />

7. Then open: Anti-spam.
We should see policies such as the default inbound anti-spam policy.
<img width="2736" height="1650" alt="7" src="https://github.com/user-attachments/assets/2dd077c9-8653-4601-9685-c4bc72c82cc7" />

8. Now lets send our test email
  Now we're going to test our rule as an actual employee.

Open a new Incognito/InPrivate window.

Open: Outlook on the web

Sign in as: Sarah Johnson
<img width="1312" height="1656" alt="8" src="https://github.com/user-attachments/assets/f6b5ac5d-9fb5-4330-be0d-af0d1dfb30e7" />

9. Now we'd Create a new email.

To: James Wilson
Subject: HR Priority Test - LAB08
Message: This is a test message to validate our Exchange Online HR mail flow rule.
<img width="1119" height="1405" alt="9" src="https://github.com/user-attachments/assets/edad694f-121a-44cc-a93d-498bb0954938" />

10.  Lets create a HR Mail Routing Rule: When Sarah Johnson from HR sends an  email, Exchange automatically adds Emily Carter in HR as a recipient.
<img width="2736" height="1628" alt="10" src="https://github.com/user-attachments/assets/be61ba95-206a-47f0-9ea7-de44cc302611" />

11. Under the "Apply rule if" 
    The sender → is this person → Sarah Johnson
    This means the rule is triggered when Sarah sends an email.
    Under "do the following"
    Add recipients → to the To box → Emily Carter
<img width="2736" height="1642" alt="11" src="https://github.com/user-attachments/assets/8f841771-d485-4c7d-b969-15b64717eb53" />

12. Here we put severity as high , and click on next to complete our new transport rule
<img width="2732" height="1660" alt="12" src="https://github.com/user-attachments/assets/783a10ec-24c2-48a3-8d93-a42cf23351d6" />

13. Confirmation of our new transport rule
<img width="2732" height="1650" alt="13" src="https://github.com/user-attachments/assets/c740c744-52ed-472e-95df-99e11bcd197c" />

14. Here we would enable our new transport rule
<img width="2736" height="1668" alt="14" src="https://github.com/user-attachments/assets/d88f39ab-07b3-46f0-a74b-505b964197d7" />

15. Here we'd Test the rule
Lets Sign into Sarah Johnson's Outlook and Create a new email to another test user — we would not manually add Emily Carter.
Subject: HR Policy Update 
Body: This is a test message to validate the HR mail routing rule configured in Exchange Online.
Now we Send it to James Wilson
<img width="2736" height="1648" alt="15" src="https://github.com/user-attachments/assets/0e5a6d2e-4c71-4bd3-b22e-1547be3f0f96" />

16. Now sign into Emily Carter's Outlook , As you can see our rule is effective as she received our email
<img width="2736" height="1620" alt="16" src="https://github.com/user-attachments/assets/d9972b54-3562-4d0d-bb9f-03c63964db2f" />

17. Let's move to the Message Trace, it proves from the Exchange administrator side that the message was processed and delivered.
Lets Open Message Trace
In the Exchange Admin Center, go to:
Mail flow → Message trace 
Then we'd click on Start a trace
<img width="1306" height="1644" alt="17" src="https://github.com/user-attachments/assets/0cbde865-3b61-4dde-9c99-c72d5199d917" />

18. Set the search criteria around the email we just tested.
Use:
Sender: Sarah Johnson
Recipient: Emily Carter
For the time range, choose something that includes when we sent the test, such as: Past 24 hours
We don't need to search the entire tenant.

Click Search.
<img width="2736" height="1654" alt="18 (2)" src="https://github.com/user-attachments/assets/a8a753df-59bb-41a1-bbf7-3a5cdb9ef54c" />

19.  As you can see , due to our HR policy  Update , our email was successfully delivered to Emily Carter in HR automatically from sarah Johnson in HR
<img width="2734" height="1650" alt="19" src="https://github.com/user-attachments/assets/519666bc-0d5e-4a5a-99d6-ac6ba7024600" />






