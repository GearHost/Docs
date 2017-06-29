# How to configure DNS records

In order for the DNS zone to work in your portal. Be sure your domain is pointed to the following name servers:

`ns1.gear.host`
`ns2.gear.host`

### How to access DNS zone editor
1. Log in to your [control portal](http://my.gearhost.com/).
2. Select the CloudSite that contains the domain you want to make DNS changes to
3. Select the **Domains** tab and then select the domain you wish to configure the DNS records for
4. You can configure any DNS record from this panel

### How to configure Office 365

###### Adding the TXT record for verification
Before you can use your domain name with Office 365, you have to verify that you own it. By being able to update the DNS zone file you are proving to Office 365 that you own the domain.

1. Select `Add Record`
2. Select `TXT` record type
3. Fill out the form with these settings
	| Enter Name  | Enter Hostname 
    | ------------- | ------------- 
    | @ | MS=msXXXXXXXX 
4. Click Create



###### Adding CNAME record
1. Select `Add Record`
2. Select `CNAME` record type
3. Fill out with the settings below
    | Enter Name  | Enter Hostname 
    | ------------- | ------------- 
    | autodiscover | autodiscover.outlook.com 
    | sip  | sipdir.online.lync.com  
    | lyncdiscover  | webdir.online.lync.com  
    | msoid  | clientconfig.microsoftonline-p.net  
    | enterpriseregistration | enterpriseregistration.windows.net
    | enterpriseenrollment | enterpriseenrollment.manage.microsoft.com

###### Adding The TXT Record For SPF To Prevent Email Spam
1. Select `Add Record`
2. Select `TXT` record type
3. Fill out the form with these settings
	| Enter Name  | Enter Hostname 
    | ------------- | ------------- 
    | @ | v=spf1 include:spf.protection.outlook.com -all 
4. Click Create

###### Adding the SRV Record

1. For the first SRV record select `Add Record`
2. Select `SRV` record type
3. Fill out the form with these settings
	| Priority  | Weight | Port  | Service Name  | Target
    | ------------- | ------------- | ------------- | ------------- | ------------- 
    | 100 | 1 | 443 | _sip._tls | sipdir.online.lync.com
    | 100 | 1 | 5061 | _sipfederationtls._tcp | sipfed.online.lync.com


>**Tip:** Unable to create a specific DNS record? All you need to do is [contact us](https://www.gearhost.com/documentation/how-to-open-a-support-ticket)!
