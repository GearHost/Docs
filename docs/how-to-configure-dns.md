# How To Configure DNS Records
In order for the DNS zone to work in your portal. Be sure your domain is pointed to the following name servers:

`ns1.gearhost.com`

`ns2.gearhost.com`

### How to access DNS zone editor
1. [Log in to your GearHost Account](https://my.gearhost.com/Account/Login)
2. Select the DNS tab on the left
3. Select the Domain you want to edit
4. You can configure any DNS record from this panel

### How to configure Office 365

###### Adding the TXT record for verification
Before you can use your domain name with Office 365, you have to verify that you own it. By being able to update the DNS zone file you are proving to Office 365 that you own the domain.

1. Select `TXT` record type

3. Fill out the form with these settings

    ​	Hostname: @ | Value: MS=msXXXXXXXX | TTL: 3600
    
4. Click Create



###### Adding CNAME record
1. Select `CNAME` record type

3. Fill out with the settings below

    ​	Hostname: autodiscover | Alias: autodiscover.outlook.com 
    ​	Hostname: sip  | Alias: sipdir.online.lync.com | TTL: 3600
    ​	Hostname: lyncdiscover  | Alias: webdir.online.lync.com | TTL: 3600
    ​	Hostname: msoid  | Alias: clientconfig.microsoftonline-p.net | TTL: 3600
    ​	Hostname: enterpriseregistration | Alias: enterpriseregistration.windows.net | TTL: 3600
    ​	Hostname: enterpriseenrollment  | Alias: enterpriseenrollment.manage.microsoft.com | TTL: 3600

###### Adding The TXT Record For SPF To Prevent Email Spam
1. Select `TXT` record type
3. Fill out the form with these settings

	Hostname: @ | Value: v=spf1 include:spf.protection.outlook.com -all | TTL: 3600
4. Click Create

###### Adding the SRV Record

1. Select `SRV` record type

3. Fill out the form with these settings

	​	Hostname: \_sip.\_tls | Target: sipdir.online.lync.com | Priority: 100 | Weight: 1 | Port: 443
	
	​	Hostname:  \_sipfederationtls.\_tcp | Target: sipdir.online.lync.com | Priority: 100 | Weight: 1 | 
	
	​	Port: 443
	
	


>**Tip:** Unable to create a specific DNS record? All you need to do is [contact us](https://www.gearhost.com/documentation/how-to-open-a-support-ticket)!
