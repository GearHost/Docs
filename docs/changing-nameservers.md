#GearHost Nameservers
We highly recommend using our nameservers as we've partnered up with [CloudFlare](https://www.cloudflare.com/ddos/dns-flood/) to mitigate DDOS attacks if such event occurs. 
For TLD root domains to work on GearHost you must point your domain's name servers to the GearHost name servers. If you have purchased your domain through GearHost this already has been done for you. However, if you use a 3rd party domain registrar then you will need to make this change with them.

Please set your nameservers to:

` ns1.gear.host`

` ns2.gear.host`

Changes can take a few hours to propagate however sometimes in rare cases you might have to wait up to 24 hours. You can confirm if propagation has been completed using [this site](https://www.whatsmydns.net/). Simply enter your domain and set the record type to NS. This will perform a search and return the name servers that are being queried globally. 


###Using Third Party DNS
If you want to use your own nameservers, you can point your domain's A record to `204.246.56.80`. If you want to use our e-mail hosting and are using third party DNS, please contact us so we can confirm which MX record you need configured.

>**Tip:** If you have any questions let us know and [open a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket).