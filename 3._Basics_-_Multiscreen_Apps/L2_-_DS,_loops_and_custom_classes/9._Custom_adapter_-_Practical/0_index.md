# 9. Custom adapter - Practical
Created Monday 21 December 2020

Prerequistes - We've added a ListView in the ``numers_activity.xml`` file.

#### Goal
Since we need to show two strings at a time(default, Miwok).

* We need a new class called [Word.java](../_ud839_Miwok/app/src/main/java/com/example/android/miwok/Word.java) as Java doesn't have a ``pair`` class.
* We need a custom layout file for the list_item.
* We need a custom adapter that works with the ``Word`` object and the ``list_item`` view.
* We also need to change the ``NumbersActivity`` class, where we need to populate the DS, and attach it to the ``WordAdapter`` and attach the adapter to the listView.



*****


#### How to do this?
To have a custom ``list_item`` view and non-primitive DS is very common. So we have a standardized approach:

1. Create a class to represent content data.
2. Create an adapter by subclassing ArrayAdapter.
3. Modify the getView() function in the custom adapter.


Done!!

*****

``list_item.xml``
	<?xml version="1.0" encoding="utf-8"?>
	<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
	    xmlns:tools="http://schemas.android.com/tools"
	    android:layout_width="match_parent"
	    android:layout_height="wrap_content"
	    android:orientation="vertical"
	    android:padding="10dp"
	    tools:text="Sample Text">
	
	    <TextView
	        android:layout_width="match_parent"
	        android:layout_height="wrap_content"
	        android:textColor="#0000ff"
	        android:textSize="16dp"
	        android:textStyle="bold"
	        tools:text="English Word" />
	
	    <TextView
	        android:layout_width="match_parent"
	        android:layout_height="wrap_content"
	        android:textColor="#008855"
	        android:textStyle="italic"
	        tools:text="Miwok Translation" />
	</LinearLayout>

