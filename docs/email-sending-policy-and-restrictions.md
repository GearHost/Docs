#Shared Email Policy, Limits, And Restrictions

GearHost utilizes a few different methods to ensure service for all our customers and to prevent compromised accounts from impacting email services. These rules and measures are in place only for shared email services like on the latest GearHost platform. 

####Throttling
---
GearHost throttles outgoing messages to 1000 per hour. After 1000 messages are sent the rest of the messages are then delayed and sent out at a rate of 1000 per hour. Throttling does not bounce or send back messages, delivery is simply delayed. We also throttle based on bandwidth at 100MB per hour. If your mailbox exceeds 100MB in one hour then messages are delayed to 100MB per hour. 

####Abuse Detection
---
In addition to throttling we also have rules in place to prevent abuse to our mail servers. 

- SMTP - Maximum of 200 connections within 10 minutes. If the limit is exceeded your IP address will be blocked for 2 hours. If you are able to receive email but not send this could be the cause.
 
- IMAP - Maximum of 200 connections within 10 minutes. If the limit is exceeded your IP address will be blocked for 2 hours.
POP - Maximum of 200 connections within 10 minutes. If the limit is exceeded your IP address will be blocked for 2 hours.

- Password - You have a maximum of 3 bad tries within 1 minute. If you attempt to login more then 3 times with the wrong password your IP will be blocked for 10 minutes.
 
- Message sending warning- This is a warning only and not an actual block. If your mailbox sends over 100 messages in a 10 minute period we may contact you to review. Again, it is just a warning to review the account to make sure it is not compromised. 

####Account hi-jack (compromised email accounts)
---

To prevent hijacked accounts from sending out spam GearHost has throttling and blocks put in place on outgoing email. A hijacked account is an email address that has been compromised, allowing a worm or other user to use it to send out spam. GearHost must block these occurrences to prevent the mail servers from becoming blacklisted. This is another method of throttling but with a permanent ban. These limits are set to allow a "normal" level of activity from a user but take action if a specific domain or account begins to send a number of emails that is greater then what would be considered standard levels.  

#####Threshold 1

Time: 10 Minutes

Number of Emails: 50

Action Taken: If a user sends more then 50 individual emails within any 10 minute time period, those emails will be placed in a holding queue for a short time on the email server. These emails will be delivered a short time later but will be delayed. 

#####Threshold 2

Time: 30 Minutes

Number of Emails: 100

Action Taken: If a user sends out more then 100 emails within any 30 minute time period, all emails from that domain will be placed in a holding queue PERMANENTLY and no other emails sent from that domain will be delivered until the user contacts GearHost and asks to be manually removed from the block list.

####Bulk mailing rules
----

You must provide a valid FROM and RETURN email address in all messages sent from your account.
All mailing lists must contain an unsubscribe function and only subscribed mailing lists are permitted from the GearHost network.
Any mailing lists being sent out must be sent during off peak hours which are, M-F 10pm - 4am mountain time, and any time Saturday and Sundays.
When sending from this list, recipients cannot see the other email addresses in the list. When you send out a mailing list, email looks like it just went to the intended recipient. This is how our mailing list is set to function.
Bulk mailing from websites

You must authenticate with a valid email address on your domain and that must be hosted with GearHost.
You must provide a valid FROM and RETURN email address in all messages sent from your account.
All mass/bulk mailings must contain an unsubscribe function and only subscribed lists are permitted from the GearHost network.
Any mailing lists being sent out must be sent during off peak hours which are, M-F 10pm - 4am mountain time, and any time Saturday and Sundays.
Password Policy

####GearHost requires the following for your email address password. 
----
- Minimum of 8 characters.
- At least one upper and one lower case character.
- At least one number.
- At least one symbol (examples: !@#$%).
- Cannot be your email address.

####Additional Action Taken

If GearHost finds a compromised account on our mail servers (detected through the methods above) we will immediately disable the email address and change the password. We will then contact the customer to let them know the email address has been compromised. 

GearHost reserves the right to terminate any mass mailing failing to meet these rules and also block future mailings. We may do this without warning and messages sent may be deleted if they are seen as spam. We will inform customers through their account contact information via email if you fail any of these rules and your messages are blocked.

#####What if I believe I am blocked?
If you believe that your email address or IP address is being blocked, please contact GearHost by opening a support ticket. In the ticket we will need the following information.

- Email address you are sending from
- IP address of your current location (http://www.whatsmyip.org can be used if you are unsure)
- GearHost will review the information and the content of the emails being sent and will either remove the block on the domain so that emails may be sent once again or contact you to review current block and what actions need to be taken.