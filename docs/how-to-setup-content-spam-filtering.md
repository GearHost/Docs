<h1>How To Setup Content &amp; Spam Filtering</h1>
<p>Before learning about how to setup your content &amp; spam filters it is also important to know <a href="https://www.spamhaus.org/statistics/tlds/">The 10 Most Abused Top Level Domains</a>. As of July 19, 2017 the TLDs with the worst reputations for spam operations are:</p>
<table style="width: 100%;">
<tbody>
<tr>
<td>1) <em>www.example</em><strong>.study</strong></td>
<td>6) <em>www.example</em><strong>.top</strong></td>
</tr>
<td>2) <em>www.example</em><strong>.party</strong></td>
<td>7) <em>www.example</em><strong>.life</strong></td>
</tr>
<tr>
<td>3) <em>www.example</em><strong>.gdn</strong></td>
<td>8) <em>www.example</em><strong>.gq</strong></td>
</tr>
<tr>
<td>4) <em>www.example</em><strong>.click</strong></td>
<td>9) <em>www.example</em><strong>.yokohama</strong></td>
</tr>
<tr>
<td>5) <em>www.example</em><strong>.accountant</strong></td>
<td>10) <em>www.example</em><strong>.ml</strong></td>
</tr>
</tbody>
</table>

<h2>Content Filtering</h2>
<p>Content filtering is a great way to perform actions on emails that meet specific criteria. For example, you can use content filters to delete messages with certain attachments (e.g., attachments with a .exe extension), forward messages from a specific email address to another account, or even alter the subject of specific types of email. Content filters are most commonly used to organize email by moving messages to specific folders. However, content filtering is extremely flexible and allows you to filter messages the way you want to.</p>
<h3>Access Content Filtering Settings</h3>
<ol>
<li><a href="https://my.gearhost.com/account/login">Log in to your GearHost Account</a></li>
<li><strong>Click</strong> on the CloudSite name you wish to manage email under</li>
<li>Click the <code>Email</code> tab</li>
<li><strong>Click</strong> the domain name you wish to manage</li>
<li>Click the <code>Email Management</code> button to launch the SmarterMail web mail interface</li>
<li><strong>Click</strong> the <code>Settings</code> gear icon on the left menu panel</li>
<li>Then expand the <code>My Settings</code> &amp; <code>Filtering</code> folders</li>
<li>Click <strong>Content Filtering</strong></li>
</ol>
<blockquote>
<p><strong>Note</strong>: If you have blocked any senders in your Inbox, there may be a content rule that was automatically created as a result of that action.</p>
</blockquote>
<h3>Add a New Filter</h3>
<ol>
<li><strong>Click</strong> <code>New</code> in the content pane toolbar</li>
<li>Fill out the content filter wizard <code>to your preference</code></li>
</ol>
<blockquote>
<p><strong>Note</strong>: For more information on the content filter wizard please direct your attention to that section in the article</p>
</blockquote>
<h3>Edit Existing Filter</h3>
<ol>
<li><strong>Select</strong> the desired filter</li>
<li>Click <code>Edit</code> in the content pane toolbar</li>
</ol>
<blockquote>
<p><strong>Note</strong>: Content filters are executed in the order in which they appear in the list. Therefore, when a content filter gets triggered and performs an action on a message, no other content filtering is performed on that message. To change the order, click on the arrows next to a filter.</p>
</blockquote>
<h3>Content Filter Wizard</h3>
<p>The Content Filter wizard is three pages long, and the wizard will walk you through each step necessary to create the filter. You can go back and forward within the wizard, and <strong>a rule will only be created when you actually Save it.</strong></p>
<h4>Step 1 - Filter Criteria</h4>
<p>In this step of the wizard, choose the type of things that the filter will look at. <strong>Multiple criteria can be chosen</strong>, and you can choose in the next step whether all criteria must be met, or only one of the criteria for the filter to activate.</p>
<blockquote>
<p><strong>Note</strong>: If you select a filter or action that requires an value to be entered and the field is left blank, SmarterMail will ignore this rule.</p>
</blockquote>
<h4>Step 2 - Filter Type &amp; Criteria Details</h4>
<p>Choose whether this filter uses the <strong>&quot;And&quot;</strong> modifier or the <strong>&quot;Or&quot;</strong> modifier. Then choose whether you will be using any <code>wildcards</code> in your search strings. Usually, wildcards will not be necessary, but there are times when some people may want them.</p>
<p>For each of the criteria you chose in step 1, you will <strong>be able to enter details</strong>. Many types of content filters allow lists of items to be entered in, and these will be indicated. For example, if you chose to filter on From Address, you can enter multiple email addresses in the box <code>(one per line)</code> and if a message is from any of them, that criteria will be met.</p>
<p>You also have the ability to reverse the logic of a specific criteria item by changing the <strong>&quot;matches&quot;</strong> box to <strong>&quot;does not match&quot;</strong> or the <strong>“yes”</strong> box to <strong>“no.”</strong></p>
<h4>Step 3 - Rule &amp; Actions</h4>
<p><strong>A summary of your content filter rule will appear near the top of the page.</strong> Check that it is filtering the way you intend, and enter a name for the rule so that you can easily identify it later.</p>
<p>Then, choose one or more actions to take when a message matches this filter. The available actions are explained below:</p>
<p><strong>Mark as read</strong> - Automatically marks the messages a read, which means it will not show up in your inbox, or any other folder, as unread.</p>
<p><strong>Mark as follow-up</strong> - Automatically flags the message for follow-up. This makes it easy to find messages that have been acted upon by your content filter.</p>
<p><strong>Delete message</strong> - Deletes the message so that it will never arrive at your Inbox. Note: Messages deleted through content filtering are not recoverable.</p>
<p><strong>Bounce message</strong> - Sends a message back to the sender of the email saying that the message was bounced. Note that the message is still delivered to you unless you choose to delete it as well. Note: If the system administrator has disabled bouncing, this option will function the same as the delete action.</p>
<p><strong>Move message</strong> - Delivers the incoming message to the folder you choose from the drop-down list. If you later delete that folder and leave the content filter active, the filter will automatically create the folder when the action is triggered.</p>
<p><strong>Prefix subject</strong> - Will append a prefix to the subject line of the email. This is useful for categorizing emails as the subject line will be altered to include the text you specify in the Comment box.</p>
<p><strong>Add Header</strong> - Includes an email header into the message, which can be useful when performing additional filtering through Outlook or another email clients. Headers should be formatted like &quot;X-someheadername: value&quot;</p>
<p><strong>Copy message</strong> - Forwards a copy of the message to another email address and leaves a copy of the message in your account as well.</p>
<p><strong>Reroute message</strong> - Forwards the message to another email address. Unlike &quot;Copy message&quot;, this option will not store a copy of the email in your own account.</p>
<p><strong>Set Priority</strong> - Will automatically elevate the priority of a message. For example, if you create a content filter that flags a message from a VIP, you may want to set the priority of the message to High as well to denote its importance.</p>
<p>Once the content filter is created, <strong>click</strong> <code>Save</code> to actually make the filter active. You can move back and forth throughout the wizard as well in order to check, and double check, your settings.</p>
<h2>Spam Filtering</h2>
<p><strong>SmarterMail includes many antispam measures that will help keep your inbox free of unwanted mail</strong>. In most cases, your system administrator, or even your domain administrator, already has some basic spam filtering options set up. However, you can certainly modify those settings to further filter out potentially unwanted email.</p>
<p>To view your spam filtering settings:</p>
<ol>
<li><a href="https://my.gearhost.com/account/login">Log in to your GearHost Account</a></li>
<li><strong>Click</strong> on the CloudSite name you wish to manage email under</li>
<li>Click the <code>Email</code> tab</li>
<li><strong>Click</strong> the domain name you wish to manage</li>
<li>Click the <code>Email Management</code> button to launch the SmarterMail web mail interface</li>
<li><strong>Click</strong> the <code>Settings</code> gear icon on the left menu panel</li>
<li>Then expand the <code>My Settings</code> &amp; <code>Filtering</code> folders</li>
<li>Click <strong>Spam Filtering</strong></li>
</ol>
<blockquote>
<p><strong>Note</strong>: The spam filtering settings will load in the content pane and the following tabs will be available.</p>
</blockquote>
<h3>Options</h3><div style="float: right;"><img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/spam_filtering.png" alt="Spam Filter"/></div>
<p>Use this tab to specify the following settings:</p>
<ol>
<li><strong>Use default spam settings</strong> - Select this checkbox to accept the default spam options provided by your domain administrator.</li>
<li><strong>Override spam settings for this account</strong> - Select this checkbox to customize the way spam is handled and to override the settings created by the domain administrator.</li>
</ol>
<h3>Actions</h3>
<p><strong>When you override the spam options</strong> set by your system administrator, you can choose the actions that are taken when email comes in that has a <strong>low, medium, or high probability of being spam</strong>. For each spam level, choose the action you wish to have taken. If you choose to add text to the subject line of messages, type the text in the box below the action drop down.</p>
<blockquote>
<p><strong>Note</strong>: If you are using the default spam options that were set up by your administrator, these settings cannot be edited.</p>
</blockquote>
<h3>Current Weights</h3>
<p>Each type of spam check has an <strong>associated weight</strong> that factors into the spam probability of a message. <strong>When an email comes in</strong>, all of the checks listed are run, and for each check that the message fails, the weight is added to the overall score of the email. <strong>The thresholds for each spam probability are examined, and the email is placed into the appropriate category.</strong></p>
<p><strong>Tip:</strong> Did we miss something or still need help? <a href="https://www.gearhost.com/documentation/how-to-open-a-support-ticket">Open a support ticket</a> and we'll be happy to assist you!</p>
