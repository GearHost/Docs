# What is .NET Core?
.NET Core is esentially a fork of the .NET Framework. It's been redesigned to offer better performance and many other features!

#### What's the benefit of using .NET Core compared to ASP.NET?
One of the main benefits is that it's cross platform. You can run your application on Windows, Linux, or MacOS.
It offers a robust Microservice Architecture, is designed for scaleable systems and high performance applications. Simply put, you can mix microservices or services developed with .NET Framework, Java, Ruby, or other monolithic technologies and immediately increase your resources.

### Publish Existing Project
1. Retrieve your publishing profile using these [steps](https://www.gearhost.com/documentation/how-to-publish-your-app-from-visual-studio)

2. When you are ready to publish select ***Build > Publish*** from the top menu



1. Select **Import Profile** near the bottom left, browse for your publishing profile and select **Open**

2. Make sure *Web Deploy* is used and not FTP

3. On the summary page below select **Configure**

   ![image2](https://github.com/GearHost/Docs/blob/master/Images/net-core-step-1.png)

4. Click the **Settings** on the left. Make sure **Deployment Mode** is set to *Self-Contained*. Click Save

![image3](https://github.com/GearHost/Docs/blob/master/Images/net-core-step-2.png)


8. Select **Publish** and your application will start deploying!

**Note:** .NET Core will not work with a free plan. The Self Contained Deployment uses over 100mb.


**Tip:** Are you looking into migrating your ASP.NET 4.5+ application to .NET Core? Be sure to check out some prerequisites found [here!](https://docs.microsoft.com/en-us/dotnet/standard/choosing-core-framework-server)