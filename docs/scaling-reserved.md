Scaling Reserved
==================

##Introduction
Your CloudSite blew up and your getting thousands of requests? That's great, we love that and we're here to help. Scaling out with reserved instances is incredibly simple and seamless. This is perfect if your blog post was just featured on TV or you need to prep your eCommerce site for the shopping season. It will provide the same experience for all visitors no matter how many are hitting the site because it provides great performance under load. 

***
##Login to the control panel and scale
1. The first thing you will need to do is [log in][login-link] to the control panel of course. 
2. After logging in click on CloudSites on the left hand menu. 
3. Now choose the CloudSite you need to scale.
4. Then click on scale. 

    ![scale][tab-scale]
 
5. After you click on scale you will be able to choose a plan to scale too. Click on reserved and then slide the scale below for how many instances you want then click on update plan. 
6. After the plan is updated your CloudSite will quickly recycle and then scale out to as many instances as you requested. 
that have a high traffic demand to run much smoother. 
***
##Nitty gritty behind the scenes
Now that you know how to scale lets look a little at what's happening. First, some explanation. 

- Plan: This is the type of compute mode you are running under. Reserved is what we are focusing on in this doc.
- Scale: Has nothing to do with weight. Scaling allows you to consume more resources in the cloud and it also allows you to consume less. So when your CloudSite is featured on a prominent blog you can grab more power from the cloud. When those visitors start to die off you can use less saving you money.  
- Reserved: Reserved is literally your own personal web node in the cloud. Your CloudSite and other customer's CloudSites will never impact performance of anyone else because your resources are dedicated to you. But you are still protected by the cloud, if the node has any issue your CloudSite will simply be moved to a new reserved node without any intervention from you. 
- Instance: Simply put this is another reserved node. Each instance takes a reserved node from our pool and gives it to you. Then our servers on the front end spread your requests out to those instances.

So what happens when you add more instances? As explained above each instance is a reserved node. When you add more to your CloudSite it gives it more web nodes to use. If you are receiving a lot of visitors at the same time you want to spread them out for performance. Adding instances does exactly that. It adds an entire server dedicated to your CloudSite. All of the requests coming to your CloudSite are spread among the number of instances you have. The most instances you have, the more requests your site can handle. 

In the real world this means a lot more performance when you have a lot of visitors at the same time. We benchmarked a wordpress blog by flooding it with 200 requests at the same time. By adding 10 instances we were able to go from 5.9 requests/second on a single instance all the way to over 60 requests/second over 10. Of course your mileage may vary depending on the type of CloudSite you have and how it is programmed.  
***
##What are instances?

####Designed for higher traffic sites

Instances disperse your site across multiple servers allowing for traffic to be directed to lower volume servers which will let your users load your site faster.

Our instances allow for sites that demand more resources to spread out their requests to multiple server clusters to allow them to function quicker. Each instance is a clustered cloud server that will serve your cloudSites applications.

If you are experiencing slow load times we highly recommend increasing the number of instances on your site.

***
####Still need help?
If you have any other questions that aren't covered in this documentation, feel free to e-mail <help@gearhost.com>.

[Login-Link]:https://my.gearhost.com/Account/Login
[tab-scale]: https://raw.githubusercontent.com/GearHost/docs/master/Images/tab-scale.png
