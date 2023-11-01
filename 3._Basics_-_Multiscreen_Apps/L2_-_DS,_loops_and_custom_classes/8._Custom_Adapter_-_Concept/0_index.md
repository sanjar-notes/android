# 8. Custom Adapter - Concept
Created Tuesday 22 December 2020

Since the ``ArrayAdapter`` doesn't know how to work with the ``Word`` class, we need to create our own adapter(called WordAdapter), i.e subclass from the ``ArrayAdapter`` class and override the ``getView`` method.
![](./8._Custom_Adapter_-_Concept/pasted_image.png)
The ListView is like the surgeon and the adapter is like the surgical technician.
![](./8._Custom_Adapter_-_Concept/pasted_image001.png)
Because we want to handle ``Word`` only, we remove the generic argument and subclass ``ArrayAdapter<Word>``. Here's the [code](../_ud839_Miwok/app/src/main/java/com/example/android/miwok/WordAdapter.java).
Check [this](https://developer.android.com/reference/android/widget/ArrayAdapter.html?utm_source=udacity&utm_medium=course&utm_campaign=android_basics) out 

