# How To Setup Content & Spam Filtering

## Content Filtering
Content filtering is a great way to perform actions on emails that meet specific criteria. For example, you can use content filters to delete messages with certain attachments (e.g., attachments with a .exe extension), forward messages from a specific email address to another account, or even alter the subject of specific types of email. Content filters are most commonly used to organize email by moving messages to specific folders. However, content filtering is extremely flexible and allows you to filter messages the way you want to.

### Access Content Filtering Settings

1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. **Click** on the CloudSite name you wish to manage email under
3. Click the `Email` tab
4. **Click** the domain name you wish to manage
5. Click the `Email Management` button to launch the SmarterMail web mail interface
6. **Click** the `Settings` gear icon on the left menu panel
7. Then expand the `My Settings` & `Filtering` folders
8. Click **Content Filtering**

>**Note**: If you have blocked any senders in your Inbox, there may be a content rule that was automatically created as a result of that action.

### Add a New Filter
1. **Click** `New` in the content pane toolbar
2. Fill out the content filter wizard `to your preference`

>**Note**: For more information on the content filter wizard please direct your attention to that section in the article

### Edit Existing Filter
1. **Select** the desired filter
2. Click `Edit` in the content pane toolbar

>**Note**: Content filters are executed in the order in which they appear in the list. Therefore, when a content filter gets triggered and performs an action on a message, no other content filtering is performed on that message. To change the order, click on the arrows next to a filter.

### Content Filter Wizard
The Content Filter wizard is three pages long, and the wizard will walk you through each step necessary to create the filter. You can go back and forward within the wizard, and **a rule will only be created when you actually Save it.**

#### Step 1 - Filter Criteria
In this step of the wizard, choose the type of things that the filter will look at. **Multiple criteria can be chosen**, and you can choose in the next step whether all criteria must be met, or only one of the criteria for the filter to activate.

>**Note**: If you select a filter or action that requires an value to be entered and the field is left blank, SmarterMail will ignore this rule.

#### Step 2 - Filter Type & Criteria Details
Choose whether this filter uses the **"And"** modifier or the **"Or"** modifier. Then choose whether you will be using any `wildcards` in your search strings. Usually, wildcards will not be necessary, but there are times when some people may want them.

For each of the criteria you chose in step 1, you will **be able to enter details**. Many types of content filters allow lists of items to be entered in, and these will be indicated. For example, if you chose to filter on From Address, you can enter multiple email addresses in the box `(one per line)` and if a message is from any of them, that criteria will be met.

You also have the ability to reverse the logic of a specific criteria item by changing the **"matches"** box to **"does not match"** or the **“yes”** box to **“no.”**

#### Step 3 - Rule & Actions
**A summary of your content filter rule will appear near the top of the page.** Check that it is filtering the way you intend, and enter a name for the rule so that you can easily identify it later.

Then, choose one or more actions to take when a message matches this filter. The available actions are explained below:

**Mark as read** - Automatically marks the messages a read, which means it will not show up in your inbox, or any other folder, as unread.

**Mark as follow-up** - Automatically flags the message for follow-up. This makes it easy to find messages that have been acted upon by your content filter.

**Delete message** - Deletes the message so that it will never arrive at your Inbox. Note: Messages deleted through content filtering are not recoverable.

**Bounce message** - Sends a message back to the sender of the email saying that the message was bounced. Note that the message is still delivered to you unless you choose to delete it as well. Note: If the system administrator has disabled bouncing, this option will function the same as the delete action.

**Move message** - Delivers the incoming message to the folder you choose from the drop-down list. If you later delete that folder and leave the content filter active, the filter will automatically create the folder when the action is triggered.

**Prefix subject** - Will append a prefix to the subject line of the email. This is useful for categorizing emails as the subject line will be altered to include the text you specify in the Comment box.

**Add Header** - Includes an email header into the message, which can be useful when performing additional filtering through Outlook or another email clients. Headers should be formatted like "X-someheadername: value"

**Copy message** - Forwards a copy of the message to another email address and leaves a copy of the message in your account as well.

**Reroute message** - Forwards the message to another email address. Unlike "Copy message", this option will not store a copy of the email in your own account.

**Set Priority** - Will automatically elevate the priority of a message. For example, if you create a content filter that flags a message from a VIP, you may want to set the priority of the message to High as well to denote its importance.

Once the content filter is created, **click** `Save` to actually make the filter active. You can move back and forth throughout the wizard as well in order to check, and double check, your settings.

## Spam Filtering
**SmarterMail includes many antispam measures that will help keep your inbox free of unwanted mail**. In most cases, your system administrator, or even your domain administrator, already has some basic spam filtering options set up. However, you can certainly modify those settings to further filter out potentially unwanted email.

To view your spam filtering settings:

1. [Log in to your GearHost Account](https://my.gearhost.com/account/login)
2. **Click** on the CloudSite name you wish to manage email under
3. Click the `Email` tab
4. **Click** the domain name you wish to manage
5. Click the `Email Management` button to launch the SmarterMail web mail interface
6. **Click** the `Settings` gear icon on the left menu panel
7. Then expand the `My Settings` & `Filtering` folders
8. Click **Spam Filtering**

>**Note**: The spam filtering settings will load in the content pane and the following tabs will be available.

### Options
Use this tab to specify the following settings:

1. **Use default spam settings** - Select this checkbox to accept the default spam options provided by your domain administrator.
2. **Override spam settings for this account** - Select this checkbox to customize the way spam is handled and to override the settings created by the domain administrator.

### Actions
**When you override the spam options** set by your system administrator, you can choose the actions that are taken when email comes in that has a **low, medium, or high probability of being spam**. For each spam level, choose the action you wish to have taken. If you choose to add text to the subject line of messages, type the text in the box below the action drop down.

>**Note**: If you are using the default spam options that were set up by your administrator, these settings cannot be edited.

### Current Weights
Each type of spam check has an **associated weight** that factors into the spam probability of a message. **When an email comes in**, all of the checks listed are run, and for each check that the message fails, the weight is added to the overall score of the email. **The thresholds for each spam probability are examined, and the email is placed into the appropriate category.**

**Tip:** Did we miss something or still need help? [Open a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket) and we'll be happy to assist you!