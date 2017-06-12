# Setup e-mail on iPhone or iPad (iOS)

This article will help setup your GearHost mailbox on your iOS device such as an iPhone or iPad. If you are having issues with your email on your device we suggest removing the current account on your iOS device and creating a new one using the steps below if using IMAP.

1. Confirm you are using the latest iOS version using this [Apple Support Document](https://support.apple.com/en-us/HT204204)
2. Launch the **Settings** app
1. Select **Mail**
1. Select **Accounts**
2. Select **Add Account**
1. Select **Other**.
1. Select **Add Mail Account**
2. Fill out your name, email address and email mailbox password as well as a description and select **Next**
3. IMAP should be selected by default, if not select it
3. Under **Incoming Mail Server** and **Outgoing Mail Server** use the same information:
	1. **Host Name**: `mail.yourdomain.com` (replace yourdomain.com with your domain name)
	2. **User name**: Your email address
	3. **Password**: Your email mailbox password
1. Select **Next** (This process can take about 2 minutes)
2. Select **Save**  


### Disable SSL

1. Launch the **Settings** app
2. Select **Mail**
3. Select **Accounts** and choose the email account that you are working with.
4. Select **Account** `email@yourdomain.com`
5. Select **Advanced**
6. Scroll until you see **Incoming Settings**
7. Turn off **Use SSL**
4. Go back to **Account**
5. Look for **Outgoing Mail Server** and select *SMTP*
6. Select your **Primary Server**
7. Turn off **Use SSL**
8. Update the **Server Port** to **587** (Use `2525` or `25` if that does not work)
9. Tap **Done** in the top right corner
10. Go back to **Account** and tap **Done** again