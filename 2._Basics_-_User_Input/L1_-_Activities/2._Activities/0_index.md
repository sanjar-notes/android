# 2. Activities
Created Wednesday 28 October 2020


* When we made the 'Just Java' app, we used a single 'activity'.
* Activity - A single focused thing that a user can do.
* An activity may have one or more screens(i.e layouts).

For example, the ConversationListActivity in Gmail consists of multiple layouts. Some of these layouts contain buttons to change the activity.	
![](./2._Activities/pasted_image.png)
Single activity but multiple screens(layouts). All the tabs viz Social, Promotions, Updates etc and their corresponding screens belong to the same activity, i.e viewing emails.

Another example of an activity is
![](./2._Activities/pasted_image001.png)

*****


* An activity is focused on a single goal. Number of screens used is irrelevant.
* Activities *contain* layouts, they are *not* layouts(screens) themselves.

Example of activities - all have a different purpose
![](./2._Activities/pasted_image002.png)

*****


* Each activity has atleast one logic file associated with it. It can be a Java or Kotlin file.
* Our activity file, called MainActivity.java was created automatically, because we had selected Empty Activity while intializing the project in Android Studio.


