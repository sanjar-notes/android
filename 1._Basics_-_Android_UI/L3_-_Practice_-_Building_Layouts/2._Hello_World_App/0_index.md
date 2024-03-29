# 2. Hello World App
Created Sunday 25 October 2020

[./_HappyBirthday](./2._Hello_World_App/_HappyBirthday)

* The package name must uniquely identify an app in the Play Store.
* Package name is actually company_domain_reversed.ApplicationName

![](./2._Hello_World_App/pasted_image.png)

*****

Which OS to target?

* Select an OS which supports your customer base. Apps are forward compatible.

![](./2._Hello_World_App/pasted_image001.png)

* Why not select the oldest OS?

Old OSs have less features.

*****

**How to create basic scaffold and see that it works?**

* Make an app with an empty activity.
* Run it.


*****

There are two ways to test an app:

1. Using a real device - The device is connected to the computer via USB cable or WiFi. To do this via USB, first make yourself a developer by tapping the build number until the message "You are now a developer" pops up. Developer Options are now available, enable them and switch on USB Debugging(allow connection when prompted on phone). Connect the USB. Select your device from Android Studio, then run the app. That's all. The WiFi method requires a plugin.
2. Using the AVD - Android Virtual Device. It is written as "<device> <OS_level> <architecture>", e.g "Nexus 5 API 21 x86". The AVD is used to manage virtual devices. To make a virtual device, go to AVD > New Device. Select the API Level and other specs, name the device. Some OS API's may be downloaded automatically. To run the app, select current device. And run.


