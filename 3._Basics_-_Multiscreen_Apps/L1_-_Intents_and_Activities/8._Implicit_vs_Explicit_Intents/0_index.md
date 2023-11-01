# 8. Implicit vs Explicit Intents
Created Saturday 21 November 2020

There are two types of Intents:

1. **Implicit Intent** - Create an implicit intent if you don't care which app component handles the intent, as long as they do it right.
	* The OS automatically(by searching the Intent filter database) chooses the app component w.r.t the action and data(optional) provided in the intent.
	* The OS provides a disambiguation option if multiple apps are capable.

![](./8._Implicit_vs_Explicit_Intents/pasted_image.png)  ![](./8._Implicit_vs_Explicit_Intents/pasted_image001.png)

* Structure of an implicit intent

![](./8._Implicit_vs_Explicit_Intents/pasted_image004.png)


* Code for implicit Intent

	Intent i = new Intent(Intent.ACTION_DIAL, Uri.parse("https://www.vogella.com/"));
	if(i.resolveActivity(getPacketManager())!=null)
		startActivity(i);

 

2. **Explicit Intent** - If you explicitly know the component that must handle the intent.
	* Explicit intents are typically used within an app as Activity files are directly accessible to the app developer.
	* We should almost never use explicit intents for 3rd party apps, since the app may not be installed.

![](./8._Implicit_vs_Explicit_Intents/pasted_image003.png) ![](./8._Implicit_vs_Explicit_Intents/pasted_image002.png)

* Structure of an explicit intent.

![](./8._Implicit_vs_Explicit_Intents/pasted_image005.png)

* Code for explicit Intents		

	Intent i = new Intent(this, ActivityTwo.class);
	startActivity(i);


*****


### Similarities between implict and explicit Intents

* Both change the screen
* Both can have extras(key, pair)


