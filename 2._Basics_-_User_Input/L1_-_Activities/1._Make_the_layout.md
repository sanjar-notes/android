# 1. Make the layout
Created Tuesday 27 October 2020


* Build a simple layout.
* Steps:
	1. Decide the views
	2. Position the views
	3. Style them

![](./1._Make_the_layout/pasted_image.png)
	<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
	    android:layout_width="match_parent"
	    android:layout_height="match_parent">
	
	    <LinearLayout
	        android:layout_width="match_parent"
	        android:layout_height="wrap_content"
	        android:orientation="vertical"
	        android:padding="16dp">
	
	        <TextView
	            android:layout_width="wrap_content"
	            android:layout_height="wrap_content"
	            android:text="Quantity"
	            android:textAllCaps="true" />
	
	        <TextView
	            android:layout_width="wrap_content"
	            android:layout_height="wrap_content"
	            android:paddingTop="16dp"
	            android:paddingBottom="16dp"
	            android:text="0"
	            android:textColor="@color/black"
	            android:textSize="16sp" />
	
	        <Button
	            android:layout_width="wrap_content"
	            android:layout_height="wrap_content"
	            android:text="Order" />
	    </LinearLayout>
	</RelativeLayout>


