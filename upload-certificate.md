#I now have my certificate files, what do I do now?
Login to your [portal](https://my.gearhost.com) and go to **Certificates.** Select **Actions** and **Upload Signed Certificate.**

Look for your domain certificate, it should look something like **www_ domain_com.crt** 

After it's uploaded click on **Actions**, select **Generate PFX** and generate a strong password. This will download a .pfx file in your local computer. 


<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/csr2.png" width="75%"/>

###What is a .PFX file?
A .PFX file would be a file that has both your www.domain.com.crt and private .key file combined. When you generate a CSR, we provide you with a CSR code and a private key that's stored on our servers.

**You may now proceed with the last [step.](https://www.gearhost.com/documentation/how-to-install-a-pfx)**