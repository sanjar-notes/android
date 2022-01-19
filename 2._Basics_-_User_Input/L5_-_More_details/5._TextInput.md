# 5. TextInput
Created Wednesday 04 November 2020

How to take text input in Android?

* ``EditText`` view is used for taking text as input. It is a subclass of TextView.


#### **Syntax in XML**

* ``EditText`` skeleton - it is a self closing tag.

	<EditText
		android:layout_width="wrap_content"
		android:layout_height="wrap_content"/>


* ``inputType`` - ``text``, ``textMultiline``, ``textCapWords``, ``date``, ``datetime``, ``number``, ``none`` [etc](https://developer.android.com/reference/android/widget/TextView#attr_android:inputType). These types can be combined using the bitwise OR (``|``) operator

![](./5._TextInput/pasted_image001.png)

* ``hint`` - text that is visible only if EditText is empty. Used as a label. It is optional.

![](./5._TextInput/pasted_image002.png)

* ``text`` - used as initial filler text. Optional. Can be overwritten.
* ``onClick`` - triggered only for a single-line text input, where the 'Enter' key acts as the submit button. Does not work for textMultiline, because the 'Enter' key acts as the newline character.
* ``selectAllOnFocus``="true", selects everything when the user focuses.


*****


#### **EditText methods**

* **getText()** - returns an 'Editable' object that contains text. Use **to_string()** to obtain text as a String, because cast does not work.
* **setInputType(int type_name)** - for setting input type. Takes int as argument. The EditorInfo class has input type constants defined in it. e.g ``EditorInfo.TYPE_CLASS_PHONE``

![](./5._TextInput/pasted_image.png)

* **setText(String)** - used to set value in the field
* **append(String)** - appends text to the field.
* **clearFocus()** - clears the focus off the field. By default focus remains on the field even after submit.


