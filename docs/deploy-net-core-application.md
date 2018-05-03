# What is .NET Core?
.NET Core is esentially a fork of the .NET Framework. It's been redesigned to offer better performance and many other features!

#### What's the benefit of using .NET Core compared to ASP.NET?
One of the main benefits is that it's cross platform. You can run your application on Windows, Linux, or MacOS.
It offers a robust Microservice Architecture, is designed for scaleable systems and high performance applications. Simply put, you can mix microservices or services developed with .NET Framework, Java, Ruby, or other monolithic technologies and immediately increase your resources.

### Getting Started
1. You will need the latest version of [Visual Studio 2017](https://www.visualstudio.com/downloads/)
2. Also the following .NET Core SDK and frameworks found [here.](https://www.microsoft.com/net/download/windows) This can also be installed through the Visual Studio Installer GUI client
3. Retrieve your publishing profile using these [steps](https://www.gearhost.com/documentation/how-to-publish-your-app-from-visual-studio)
4. Inside Visual Studio select **File** > **New** > **Project** and click on **Web** > **ASP.NET Core Web Application**
5. Select **OK** twice 
6. Once you're ready to publish, right click on your web application project inside **Solution Explorer** and select **Edit "yourwebapplication.csproj"**
7. On top of the `<TargetFrameWork>` section add the following:
   `<RuntimeIdentifiers>win10-x64</RuntimeIdentifiers>`

8. Your .csproj file should look like this:

![image](https://raw.githubusercontent.com/GearHost/Docs/master/Images/net-core-csproj.png)


8. Save your changes. Right click your project again, and select **Publish**
9. Select **Import Profile** as the option, browse for your publishing profile and select **Open**
10. Select **Publish** and your application will start deploying!


**Tip:** Are you looking into migrating your ASP.NET 4.5+ application to .NET Core? Be sure to check out some prerequisites found [here!](https://docs.microsoft.com/en-us/dotnet/standard/choosing-core-framework-server)