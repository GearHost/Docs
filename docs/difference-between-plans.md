# Difference Between Plans
GearHost offers three different plans for your CloudSite:

-
- **Hobby**
- **Small**
- **Medium**
- **Large**

Both the free and Hobby work the same technically behind the scenes but the free plan has a lot of restrictions in place since it's meant for non production development and testing. The reserved plan is your own private node in the cloud that you can scale out further into your own private cloud so to speak. In this doc we'll go in depth over the differences between each plan and how to scale between them.  

## Comparison

	|                	| Hobby         	| Small    	     | Medium         	| Large    	     |
	|----------------	|----------------	|-------------	 |----------------	|-------------	 |
	| CPU            	| 240 min/day    	| Unlimited   	 | 240 min/day    	| Unlimited   	 |
	| RAM            	| 1024MB/hour    	| 2048MB/hour 	 | 1024MB/hour    	| 2048MB/hour 	 |
	| Storage (SSD)  	| 1GB up to 100gb 	| 1GB up to 100gb| 1GB up to 100gb 	| 1GB up to 100gb|
	| Bandwidth      	| 1TB           	| 1TB         	 | 1TB           	| 1TB         	 |
	| Requests       	| 1000 Concurrent 	| Unlimited   	 | 1000 Concurrent 	| Unlimited   	 |
	| Idle Time      	| 60 min         	|              	 | 60 min         	|              	 |
	| SSL            	| Yes            	| Yes          	 | Yes            	| Yes          	 |
	| Custom Domains 	| Yes            	| Yes          	 | Yes            	| Yes          	 |
	| Web Sockets    	| Yes            	| Yes         	 | Yes            	| Yes         	 |
	| 64-bit         	| Yes            	| Yes         	 | Yes            	| Yes         	 |
	| CPU Burst      	| 3m @ 50% / 5m  	| Unlimited   	 | 3m @ 50% / 5m  	| Unlimited   	 |

## Definitions
- CPU: The amount of CPU time your CloudSite can consume in a 24 hour period.
- RAM: The amount of node memory your CloudSite can consume per hour. 
- Storage: The amount of disk space your CloudSite can consume in the cloud. 
- Bandwidth: The amount of data your CloudSite can send out in a 24 hour period.
- Requests: The amount of requests your CloudSite is allowed to process at the same time or concurrently. 
- Idle Time: The amount of time your CloudSite can sit with no requests before it is shut down. 
- SSL: Whether or not the plan supports certificates used to encrypt data sent between clients and the nodes or cloud. 
- Custom Domains: Whether or not you can add fully qualified domains (gearhost.com is a fully qualified domain name for example) to your CloudSite. 
- Web Sockets: Whether or not the CloudSite plan allows for web sockets, a TCP based technology that allows communication between clients and servers. 
- CPU Burst: The percentage of CPU power your CloudSite is allowed to consume to in a 5 minute period. 

## Which is right for me?
There is an easy way to separate the plans. 

- **Free**: Is meant for non production web sites and applications such as development demos. 
- **Hobby**: Use this plan for production websites and applications. 
- **Small**: A plan that provides dedicated resources that can be scaled out. If you have an application that is growing rapidly or that you expect significant traffic this is the most powerful plan. It can also be scaled out with multiple instances to create a private web farm. 

Fortunately, you don't even have to make this decision now. You can start with free and then scale up if you run into limits. Same thing with standard and reserved allows you to scale out across multiple instances. Each instance is a private node in the cloud. 

#### Still need help?
If you have any other questions that aren't covered in this document, feel free to e-mail <help@gearhost.com>.