# 3. Relation between Java and XML
Created Tuesday 03 November 2020

How do Java and XML work together to create an app experience.

* When the app is run, some initialization takes place and the MainActivity.java file is run.
* Its onCreate function accesses the layout from the activity_layout.xml file.
* This XML file is parsed and a hierarchy tree is created in memory.
* The tree is rendered on the display.
* The nodes of the tree consist of objects called views, and they can be manipulated by the Java file. These objects have attributes which can be manipulated using their functions.

![](./3._Relation_between_Java_and_XML/pasted_image.png)

*****

All views are objects.

![](./3._Relation_between_Java_and_XML/pasted_image001.png)

