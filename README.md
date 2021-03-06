# Azure Notification Hubs Sample

## :white_medium_square: Table of contents
* [What is this?](https://github.com/saramgsilva/NotificationHubs#white_medium_square-what-is-this)
* [Requirements](https://github.com/saramgsilva/NotificationHubs#white_medium_square-requirements)
* [Sample Status](https://github.com/saramgsilva/NotificationHubs#white_medium_square-sample-status)
* [The Source Code](https://github.com/saramgsilva/NotificationHubs#white_medium_square-the-source-code)
* [Screenshots](https://github.com/saramgsilva/NotificationHubs#white_medium_square-screenshots)
* [Resources](https://github.com/saramgsilva/NotificationHubs#white_medium_square-resources)
* [Common Issues](https://github.com/saramgsilva/NotificationHubs#white_medium_square-common-issues)
* [Tips](https://github.com/saramgsilva/NotificationHubs#white_medium_square-tips)
* [Build the project](https://github.com/saramgsilva/NotificationHubs#white_medium_square-build-the-project)
* [Contributors](https://github.com/saramgsilva/NotificationHubs#white_medium_square-contributors)
* [Contribute](https://github.com/saramgsilva/NotificationHubs#white_medium_square-contribute)
* [License](https://github.com/saramgsilva/NotificationHubs#white_medium_square-license)

## :white_medium_square: What is this?

The sample provided has the goal to help developers add Push Notifications to their applications, through [Azure Notification Hubs](http://azure.microsoft.com/en-us/documentation/services/notification-hubs/) and this sample supports the two main ways to manage devices in Azure Notification Hubs:

* Case 1 - Devices register directly in Azure Notification Hubs 
* Case 2 - Devices register in Azure Notification Hubs through backend


## :white_medium_square: Requirements


* Create the Azure Notification Hubs in Azure Portal (Azure Mobile Service create it by default)
* Create the required data, in Push Notification Service (WNS, GCM, APNs...), to support push notification for each Platform
* Configure the Azure Notification Hub, in Azure Portal, with the data from Push Notification Services (WNS, GCM, APNs...)
* Add connection string and hub name from the Azure Notification Hub created (in the sample it is defined in [Contants.cs file](https://github.com/saramgsilva/NotificationHubs/blob/master/Shared/Constants.cs))


## :white_medium_square: Sample Status


* **Key:** :white_check_mark: = Supported,  :x: = Not Supported, :wrench: = In development 

##### Windows Applications - Using XAML / CSharp

Platform | Case 1 | Case 2 using WebAPI (V1) | Case 2 using WebAPI (V2) | Case 2 using AMS (V2) 
:---------- | :------------------------ | :------------------------ | :------------------------ | :------------------------ |
Windows Store 8.1 (WinRT) | :white_check_mark:  | :white_check_mark: | :white_check_mark: | :white_check_mark: 
Windows Phone 8.1 (WinRT) | :white_check_mark: | :white_check_mark:   | :white_check_mark:   | :white_check_mark:
Windows Phone 8.1 (SL)| :white_check_mark: | :white_check_mark: | :white_check_mark:| :white_check_mark:


##### Windows Applications - Using XAML / Visual Basic

Platform | Case 1 | Case 2 using WebAPI (V1) | Case 2 using WebAPI (V2) | Case 2 using AMS (V2) 
:---------- | :------------------------ | :------------------------ | :------------------------ | :------------------------ |
Windows Store 8.1 (WinRT) | :white_check_mark:  | :white_check_mark: | :white_check_mark: | :white_check_mark: 
Windows Phone 8.1 (WinRT) | :white_check_mark: | :white_check_mark:   | :white_check_mark:   | :white_check_mark:
Windows Phone 8.1 (SL)| :white_check_mark: | :white_check_mark: | :white_check_mark:| :white_check_mark:

##### Xamarin Applications

Platform | Case 1 | Case 2 using WebAPI (V1) | Case 2 using WebAPI (V2) | Case 2 using AMS (V2) 
:---------- | :------------------------ | :------------------------ | :------------------------ | :------------------------ |
Xamarin Android | :white_check_mark: | :white_check_mark:  | :white_check_mark:   | :white_check_mark: 
Xamarin IOS | :wrench: | :wrench:| :wrench:| :wrench:

#### Others

Platform | Case 1 | Case 2 using WebAPI (V1) | Case 2 using WebAPI (V2) | Case 2 using AMS (V2) 
:---------- | :------------------------ | :------------------------ | :------------------------ | :------------------------ |
Android Native |  :wrench:  | :wrench:| :wrench: | :wrench:
IOS Native | :white_check_mark:   | :wrench:| :wrench:| :wrench:
Cordova |  :x:   |  :x:  |  :x:  |  :x:  


:warning: Notes:


1. The Case V1 was created in June 2014 following the documentation, but it changed and the Case 2 V2 was created to show the new version. At the end all version will work and for example the Azure Mobile Services will uses a solution similar to the Case 2 V1.

2.  The Windows Phone 8.0 implementation is similar to Windows Phone 8.1 SL implementation, this way it will not be provided.

3. For Cordova apps, see the article [MSDN Magazine - Push Notifications to Cordova Apps with Microsoft Azure](http://msdn.microsoft.com/en-us/magazine/dn879353.aspx) by [Glenn Gailey](http://msdn.microsoft.com/en-us/magazine/dn879353.aspx).



## :white_medium_square: The Source Code


### Windows and Xamarin applications


The solution has three main folders:
* Shared: contain the files shared between projects
* Case 1 - Devices register directly in Azure Notification Hubs: contain all projects related with the Case 1
* Case 2 - Devices register in Azure Notification Hubs through backend: contain all projects related with the Case 2

<MTMarkdownOptions output='html4'>
<img align="middle" src="https://raw.githubusercontent.com/saramgsilva/NotificationHubs/master/ScreenShots/FinalSolution-Opened.png"> 
</MTMarkdownOptions>  

> All projects for Windows and Xamarin using C#

Read more about the solution in the respective [source code page](https://github.com/saramgsilva/NotificationHubs/tree/master/src).


## :white_medium_square: Screenshots


The [Sceenshots folder](https://github.com/saramgsilva/NotificationHubs/tree/master/ScreenShots) contains image for each platform provided.

<MTMarkdownOptions output='html4'>
<img align="middle" src="https://raw.githubusercontent.com/saramgsilva/NotificationHubs/master/ScreenShots/Windows%20Sample%20-%201%20-%20Registration%20&%20Notification.png"> 
</MTMarkdownOptions>  


## :white_medium_square: Resources


* [MSDN Documentation] (http://msdn.microsoft.com/en-us/library/jj891130.aspx)

* [Curah! Azure Notification Hubs] (https://curah.microsoft.com/72603/notification-hubs)

* [Azure Notification Hubs– All resources you need](http://www.saramgsilva.com/index.php/2014/azure-notification-hubs-all-resources-you-need/) 

* Presentation

<MTMarkdownOptions output='html4'>
<a href="http://www.saramgsilva.com/index.php/2014/mobile-notification-for-any-device-using-azure-notification-hubs/" target="_blank"><img align="middle" src="http://s20.postimg.org/xt7iab6jh/presentation.png"> </a>
</MTMarkdownOptions>  



## :white_medium_square: Common Issues

The following list provide some common issues I found when I did the sample or even when help others developers.

### In General  

* The connection string from Notification Hubs is wrong;
* The xml/json that define the template are not well defined;
* When debug the notification is not using the correct tag or forget to use the tag;
* Is missing the configurations in Azure Portal for each application;
* In Azure Mobile Services developers uses the Notification Hubs API to manage devices and it is not necessary because Azure Mobile Service give us it out-of-box;
* When developers implement the registration in devices do not use the debug feature to verify if the devices was registered correctly; 
* Developers implements the Case 1 when they want to implement the Case 2 and mixes the two cases;

### In Windows (WinRT) apps:

* In manifest should be defined the Toast capable;
* In manifest should be defined the Internet capability;
* Associate with store;

### In Windows Phone (SL) apps:

* In manifest should be defined Internet capability, Toast capable and the ID_CAP_PushNotification
* Should be handled the notification when the app is running

### In Android apps:

* The Project Id is wrong;
* The GCM component is missing;
* In debug mode, after stop the debug be aware that is need to run again the app to receive the notifications;
* The manifest file must have the package's name starting with lower case;
* The key used in the payload is not the same in the application;


## :white_medium_square: Tips


### Push Notification Service by Platform

Platform | Push Notification Service 
:---------- | :------------------------ 
Windows Store 8.1 (WinRT) | Windows Push Notification Services (WNS) 
Windows Phone 8.1 (WinRT) | Windows Push Notification Services (WNS)
Windows Phone 8.1 (SL)| Microsoft Push Notification Service (MPNS)
Windows Phone 8.0 (SL)| Microsoft Push Notification Service (MPNS)
Android | Google Cloud Service (GCM)
IOS | Apple Push Notification Service (APNs)



### Development In Xamarin.Android

If you are using simulator and do the deploy for install the app or debug it, you can receive Push Notification while the app run, but if you stop and try to send another Push Notification the simulator will not receive it, you should run again the app without VS to get the push notification



## :white_medium_square: Build the project


To develop on this project, just clone the project to your computer, package restore is enable so build the solution first, if you get any errors try to build again and if necessary close the solution and open again to load the references.



## :white_medium_square: Contributors


<MTMarkdownOptions output='html4'>
     	<a href="https://twitter.com/saramgsilva"><img src="http://saramgsilva.github.io/NotificationHubs/images/Eu_400x400.png" height="50"/></a>
		<a href="https://twitter.com/paulomorgado"><img src="http://saramgsilva.github.io/NotificationHubs/images/PauloMorgado_320x240_400x400.jpg" height="50"/></a>
		<a href="https://twitter.com/adpead"><img src="http://saramgsilva.github.io/NotificationHubs/images/gn8frj8ipi0rsntcvcd0_400x400.jpeg"/ height="50"></a>
		<a href="https://twitter.com/clerigo"><img src="http://saramgsilva.github.io/NotificationHubs/images/EbslN-rW_400x400.jpeg"/ height="50"></a>	</p>
</MTMarkdownOptions>  


## :white_medium_square: Contribute


Everbody is welcome to contribute, only is required to provide all cases to manage devices in [Azure Notification Hubs](http://azure.microsoft.com/en-us/documentation/services/notification-hubs/).

Twitter hashtag : [#notificationhubs](https://twitter.com/search?q=%23notificationhubs&src=typd)


## :white_medium_square: License


MIT License (MIT), read more about it in the [LICENSE file](https://raw.githubusercontent.com/saramgsilva/NotificationHubs/master/LICENSE.txt).


