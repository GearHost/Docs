# General Client Email Settings

The Settings below are universal and should apply to most, if not all email clients.  We do have step by step guides for popular platforms such as Android, iOS and Windows you can read through as well if you need a more detailed walk through. 

### Desktop Settings:
**General**

Account/Username: **user@yourdomain.com**  
**Password**: Password to email account above

**IMAP**:

Port: **143**  
Security type: **None/SSL off**

**POP3**:

Port: **110**  
Security type: **None/SSL off**


**Incoming and outgoing**:

Server (SMPT): **mail.yourdomain.com**  
Outgoing server requires authentication (use same as incoming)
Port: **2525** (use 587 if this does not work)  
Security type: **None/SSL off**

### Mobile Settings:
**General**

Account/Username: **user@yourdomain.com**  
**Password**: Password to email account above

**IMAP**:

Port: **143**  
Security type: **None/SSL off**

**POP3**:

Port: **110**  
Security type: **None/SSL off**

**Incoming and outgoing**:

Server (SMPT): **mail.yourdomain.com**  
Outgoing server requires authentication (use same as incoming)
Port: **587** (use 2525 if this does not work)  
Security type: **None/SSL off**

### Using SSL for Shared Email
If you wish to use an SSL when you connect you will need to substitute the above server and port settings for the ones below.

Server: **mail#.gearhost.com** (Replace #  with the mail server number your mail is on)

**Incoming:**

IMAP Port: **993**  
POP3 Port: **995**


**Outgoing:**

SMTP Port: **465**

### Difference between IMAP and POP3
**POP3** | Post Office Protocol

- You can use only one computer to check your email (no other devices)
- Your mails are stored on the computer that you use
- Sent mail is stored locally on your PC, not on a mail server

**IMAP** | Internet Messaging Access Protocol

- You can use multiple computers and devices to check your email
- Your mails are stored on the server
- Sent mail stays on the server so you can see it from any device.