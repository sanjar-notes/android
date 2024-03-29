# 7. Use an Intent to open another Activity
Created Saturday 21 November 2020


* Activities started by an activity are called sub-activities. This wording makes it easier to describe activities.
* Code for starting an in-app Activity using an Intent

	Intent i = new Intent(this, ActivityTwo.class); // (Context, ActivityClass)
	startActivity(i);


* This runs ActivityTwo class, which becomes the new screen on top of the parent activity.
* Notice that we provided 'this' as context, which helps the app track activities. As contexts are stored in a stack - it allows the user to return to the previous Activity by pressing the 'Back' button. **Nice, we didn't have to program that and it makes using the app very intuitive.**


*****


Explicit and Implicit Intents
-----------------------------

There are two kinds of intents:

1. Explicit - We explicitly provide the Activity(the destination) in the Intent itself. It's deterministic, as there's no decision made by the OS.
	* Explicit intents are typically used within an app, as classes within the app are directly accessible to app developer.
	* Code for explicit Intents

	Intent i = new Intent(this, ActivityTwo.class);
	i.putExtra("Value1", "This value one for ActivityTwo ");
	i.putExtra("Value2", "This value two ActivityTwo");
	startActivity(i);


2. Implicit - the OS automatically(by searching the Intent filter database w.r.t the given action and data URI) chooses a capable app activity.
	* The OS provides a disambiguation prompt if multiple apps are capable.
	* Code for implicit Intent

	Intent i = new Intent(Intent.ACTION_DIAL, Uri.parse("https://www.vogella.com/"));
	if(i.resolveActivity(getPacketManager())!=null) // we need to check if a capable is installed
		startActivity(i);

#### **Intents as event triggers**

* Intents can be used to send broadcast messages into the Android system. A broadcast receiver can register to an event and is notified if such an event is sent.
* An app can register to system events, like "email has arrived", "system boot complete" or  "incoming phone call" and do something accordingly.


