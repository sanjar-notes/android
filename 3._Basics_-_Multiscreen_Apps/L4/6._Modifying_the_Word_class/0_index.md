# 6. Modifying the Word class
Created Sunday 03 January 2021

We just need an image. 

* One idea is to store the image as a file, but this is not a good idea because our code is not stored as is after installing the app.
* Even if this was possible it would be inefficient in terms of space. It is better if we use a reference.
* The correct approach is to store the image's resource_name. It is just an ``Integer`` so it is very easy to work with.

![](./6._Modifying_the_Word_class/pasted_image.png)zxcb

#### Changes to the code

* ``private Integer image``
* ``public Integer getImageResourceId()``
* Add, not replace the constructor. We are doing this because phrases have no image. So it is better not to mention images while working with them.




