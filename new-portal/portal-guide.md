# Portal Guide

The new GearHost control panel organizes hosting around CloudSites. A
CloudSite brings a domain and its web, email, and DNS services together so
you can manage them from one place.

## Find your way around

| Area | What you can do |
|------|-----------------|
| **Dashboard** | See your account and service overview. |
| **CloudSites** | Create a site and open the services connected to its domain. |
| **Web** | Manage website settings, deployment details, files, SSL, and backups when available. |
| **Email** | Manage mailboxes and email settings connected to a CloudSite. |
| **Files** | Browse and manage files for supported web services. |
| **DNS** | Review and update DNS records for hosted zones. |
| **Databases** | Create and manage available SQL Server and MySQL databases. |
| **Support** | Use the support options enabled for your account. |
| **Billing** | Review available service, invoice, and payment information. |
| **Activity** | Review recent account and service events. |
| **Settings** | Manage account and security settings. |

Some areas appear only when the related service is enabled for your account.

## Work with a CloudSite

### Create one

Open **CloudSites**, select **Create CloudSite**, enter a domain, and choose
one or more services. Web Hosting, Email, and DNS can be selected together
or added according to the choices shown in the control panel.

### Manage web hosting

Open the CloudSite and select **Web**. Use the values displayed for that site
when connecting by FTP or another supported deployment method. Do not copy
connection details from another site.

The web area can also show runtime settings, site status, usage, SSL,
backups, and deployment information. Features that are still being tested
may not appear for every plan or service configuration.

### Manage DNS and SSL

Use **DNS** to review the records hosted by GearHost. DNS changes can take
time to propagate outside the control panel.

Review the SSL status after the domain points to GearHost. Do not assume a
new or migrated site is ready for production traffic until both DNS and SSL
show the expected status.

### Manage email

Use **Email** from the CloudSite or main navigation to work with the email
service attached to that domain. The available mailbox and domain controls
depend on the services enabled for the CloudSite.

### Manage databases

Use **Databases** to view the database engines available to your account.
When you create a database, store its generated credentials securely and
use the connection details shown by the control panel.

## Existing GearHost services

The new control panel and the existing control panel are separate during the
launch preview. Your existing services will not move just because you create
or sign in to a new account. GearHost will contact customers before moving
existing services.

If you create a new service in the launch preview, treat it as a separate
service unless GearHost Support has confirmed otherwise.

## Get help

Use **Support** in the control panel when it is available for your account,
or email [support@gearhost.com](mailto:support@gearhost.com).
