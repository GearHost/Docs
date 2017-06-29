# Enable SSL
Installing an SSL certificate on your website makes it more secure by encrypting communication between the server and the client. In this guide, we'll show you the required steps to follow depending on how you decide to enable SSL on your website. 


#### Prerequisites

1. [Login to your account](https://my.gearhost.com)
2. Select the **Certificates** menu on your left hand side
3. Click on `Create Certificate` button at the top right
4. Select one of the options below to enable a certificate on your website

### Order your SSL through GearHost
Ordering a certificate through GearHost makes the process faster, it's 100% automated, and ensures that it's properly installed. Our [SSL partner](https://www.digicert.com/welcome/why-choose-digicert.htm) offers one of the biggest warranties of any certificate authority at $1 million!

1. Select `I want to order a SSL certificate through GearHost`
2. Select the desired certificate and amount of years you would like applied
3. Fill out the requested hostname you want the certificate for and legal address information.

>Your order will start processing and you'll receive an e-mail from [Digicert](https://www.digicert.com/about-digicert.htm). Please check for their e-mail and approve the order. It's possible that they may contact you asking for additional verification.

### I want to generate a CSR
A Certificate Signing Request is a message sent from an applicant to a certificate authority (SSL vendor). After providing the CSR to your SSL vendor, they will provide you with a SSL certificate file.

1. Select `I want to generate CSR`
2. Fill out the requested CSR contact information 
3. Click on **Actions** on the drop down menu and select **View Certificate** to view your CSR
4. Provide CSR information to your SSL vendor.
5. Select the `Upload Signed Certificate` option
6. Browse for the certificate file your SSL vendor has provided you
 

### Upload your own certificate 
You can install your own certificate, but it will require a PFX format as that includes both your certificate and private key. After uploading your PFX, your website will automatically load it your certificate.

1. Select `I want to upload a certificate (PFX)`
2. Click on `Choose file` and browse for your PFX file
3. Enter the certificate's password 


### Generate a certificate using Let's Encrypt
[Let's Encrypt](https://letsencrypt.org/about/) is an uprising project from Silicon Valley helping secure the world wide web for everyone! Tech giants such as Google, Facebook, Cisco, Sucuri, and more are sponsoring this project to reach a major milestone for the internet world.

1. Select `I want to generate SSL certificate with Let's Encrypt`
2. Click on the domain box field and select your domain
3. Wait a couple of minutes for your certificate to fully process.

> While it's a low cost alternative, this certificate expires every 90 days. The Small CloudSite plan offers a feature were this certificate can be automatically re-generated for you! **Let's Encrypt Certificates are only available for Hobby CloudSites or higher.**

**Tip:** Did we miss something or still need help? [Open a support ticket](https://www.gearhost.com/documentation/how-to-open-a-support-ticket) and we'll be happy to assist you!
