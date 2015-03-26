##General client email settings

The Settings below are universal and should apply to most, if not all email clients.  We do have step by step guides for popular platforms such as Android, iOS and Windows you can read through as well if you need a more detailed walk through. 

-- 

###Desktop Settings:


**General**

Account/Username: user@yourdomain.com Password: Password to email account above

**Incoming**

Server: mail.yourdomain.com

**IMAP**: 
Port: 143  
Security type: None/SSL off    

**POP3**: 
Port: 110
Security type: None/SSL off

**Outgoing**:

Server (SMPT): mail.yourdomain.com
Outgoing server requires authentication (use same as incoming)

Port: 25 (use 2525 if this does not work)
Security type: None/SSL off
 ---

###Mobile Settings:


**General**

Account/Username: user@yourdomain.com Password: Password to email account above

**Incoming**

Server: mail.yourdomain.com

IMAP:
Port: 143 
Security type: None/SSL off

POP3:
Port: 110 
Security type: None/SSL off

**Outgoing**

Server (SMTP): mail.yourdomain.com
Outgoing server requires authentication/sign-in (use same as incoming)

Port: 587 (use 25 or 2525 if this does not work)
Security type: None/SSL off
 
---
**Using SSL for Shared Email**

If you wish to use an SSL when you connect you will need to substitute the above server and port settings for the ones below.

 

Server: mail#.gearhost.com (Replace # with the mail server number your mail is on.

Note: You can use a DNS lookup such as who.is to get this info from the MX record or contact us for assistance.)

**Incoming:
**
IMAP Port: 993 
POP3 Port: 995


**Outgoing:**

SMTP Port: 465

