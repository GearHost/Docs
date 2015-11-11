#Providing the CSR to your vendor and uploading your certificate.
In this section you will be able to provide the CSR code and other information to your SSL vendor. As well as uploading your certificate through your hosting portal. Here would be the most common questions they ask for. 

**What type of server should I pick?**

It would be Microsoft IIS 7+.

**SHA-1 or SHA-2?** 

SHA-2.

**How do I authenticate?**

One common option is to create the e-mail account **admin@yourdomain.com**. They will send you an e-mail for you to approve of the request. The other alternative is they will have you upload a file in your root directory 
**(/wwwroot/)** for them to verify that you're indeed the domain owner. Pick whatever option is easier for you. If you have any issues with this step, it would be best to contact them directly. 

###I've done as requested and submitted my order, what now?

After they're done verifying the domain, they will eventually proceed with e-mailing your the certificate (SSL) after it's been issued. Once you receive their SSL attachments, please proceed with the guide.

----------


##I now have my certificate files, what do I do now?
Login to your [portal](https://my.gearhost.com) and go to **Certificates.** Select **Actions** and **Upload Signed Certificate.**

Look for your domain certificate, it should look something like **www_ domain_com.crt** 

After it's uploaded click on **Actions**, select **Generate PFX** and generate a strong password. This will download a .pfx file in your local computer. 


<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/csr2.png" />

###What is a .PFX file?
A .PFX file would be a file that has both your www.domain.com.crt and private .key file combined. When you generate a CSR, we provide you with a CSR code and a private key that's stored on our servers.

###You may now proceed with the last [step.](http://example.org)