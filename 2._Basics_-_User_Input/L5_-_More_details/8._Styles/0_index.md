# 8. Styles
Created Thursday 05 November 2020


* If we have the same attributes in multiple headers(elements) in the XML, it undermines the DRY principle. To avoid it, we use styles.
* Styles also helps in separating design and content.


#### Style details

* Styles are stored in the **res/values/** directory. Style files can be named anything, but they should be XML files. 
* A **style** contains **item** elements inside it, which is enclosed inside a single root **resources** element.
* The **style **tag has two attributes:
	* *name* - name which will be used in Java/XML files.
	* *parent* - specified only if the style inherits from other styles.
* An **item** tag has two things:
	* a *name* attribute indicating the attribute the item specifies.
	* content of the tag - value which will be applied.

	<?xml version="1.0" encoding="utf-8"?>
	<resources>
		<style name="CodeFont" parent="@android:style/TextAppearance.Medium">
			<item name="android:layout_width">fill_parent</item>
			<item name="android:layout_height">wrap_content</item>
			<item name="android:textColor">#FF0000</item>
			<item name="android:layout_width">fill_parent</item>
		</style>
	</resources>

Note: Styles reside in the **res/values/** folder, so styles can be localized. They are specified in a style.xml file.

#### Using styles
Just add the style attribute.
	<TextView
		android:layout_width="match_parent"
		android:layout_height="wrap_content"
		android:textColor="#00FF00"
		android:typeface="monospace"
		android:text="@string/hello" />
	
	<!-- With style - CodeFont.xml -->
	
	<TextView
		style="@style/CodeFont"
		android:text="@string/hello" />

Note: 

* the style attribute does not need a namespace.


