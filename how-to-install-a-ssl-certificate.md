#Installing your SSL

Please note that you must have your certificate in a **.pfx** file format for the certificate to be imported and attached to your account. If you're not on this step yet, please refer to the following [guide.](https://www.gearhost.com/documentation/SSL-installation)

1. Click on **Cloudsites** from the menu, and select your cloudsite.
 
3. Click on the **SSL** tab and  **Add Certificate.**

5. Select **Attach Certificate**, browse for your .PFX file and provide the password. 

6. Click **Upload** and go to **SSL bindings** to update your certificate to match your domain.


<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/csr3.png" width="75%" />

----------


You will have to restart your application pool by going to the **Overview** tab. After that's done, your SSL should start working and you can verify by visiting https://yourdomain.com on your browser.

<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/csr4.png" /> 


----------
If you have any issues or concerns regarding your installation, please feel free to contact us anytime or open a ticket directly from your portal by clicking on the **Support** menu. 