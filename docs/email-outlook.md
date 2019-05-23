## Setting up Outlook
1. If this is your first time opening Outlook 2013 and you have not already configured an email account, you should be presented with the Add New Account screen. If not, click on the File tab and then click on Account Settings.

	![step-1]

2. On the Account Settings page click the E-Mail Tab and select New...

	![step-2]

3. On the Add New Account window, click on the bubble next to Manually configure ... and click Next.

	![step-3]

4. Now choose POP or IMAP.

	![step-4]

5. Fill in the form as indicated below.

**User Information**

*Your Name:* Your name you would like displayed when sending email. 

<!--This can be your full name, or even a company name if this is a common mailbox like sales or billing.--> 

*E-mail address:* This is the FULL email address you are trying to add.

**Server Information**

*Account Type:* POP3 or IMAP. 
We recommend choosing IMAP.

*Incoming mail server:* mail.your-domain-name.com 

*Outgoing mail server (SMTP):* mail.your-domain-name.com 

> Replace your-domain-name with your domain name. The domain name is the part of your email address after the @ symbol. For example, if your email address is joe@example.com then the domain name is example.com and the incoming and outgoing mail servers would be mail.example.com. 

**Logon Information**

*User name:* The email address you are configuring in Outlook 2013. 

*Password:* The password to your email address.

**Do not check the box next to require logon using secure password authentication (SPA).**

![step-5]

6. After you fill in the information click on the more settings button and then click on the Outgoing Server tab. Check the box next to My Outgoing server requires authentication and use same settings as incoming mail server.

	![step-6]

7. Click Ok and click on the Test Account settings button. If everything is ok, then click Next to complete the setup. If you fail to send the test message, continue to step 7.

	![step-7]

8. if you failed to send the test message, try changing your outgoing port to our alternative 2525. Some internet service providers do not allow traffic out on port 25 (the default SMTP port) to prevent spam. Changing the port can get around this.

Click on the more settings button again and then click on advanced.
Change the SMTP port to 2525.

![step-8]

Setup is now complete and email should start syncing.

[step-1]: https://raw.githubusercontent.com/GearHost/docs/master/Images/email-outlook-step1.png
[step-2]: https://raw.githubusercontent.com/GearHost/docs/master/Images/email-outlook-step2.png
[step-3]: https://raw.githubusercontent.com/GearHost/docs/master/Images/email-outlook-step3.png
[step-4]: https://raw.githubusercontent.com/GearHost/docs/master/Images/email-outlook-step4.png
[step-5]: https://raw.githubusercontent.com/GearHost/docs/master/Images/email-outlook-step5.png
[step-6]: https://raw.githubusercontent.com/GearHost/docs/master/Images/email-outlook-step6.png
[step-7]: https://raw.githubusercontent.com/GearHost/docs/master/Images/email-outlook-step7.png
[step-8]: https://raw.githubusercontent.com/GearHost/docs/master/Images/email-outlook-step8.png