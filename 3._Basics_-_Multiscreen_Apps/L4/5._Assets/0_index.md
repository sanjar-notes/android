# 5. Assets
Created Sunday 03 January 2021


* Assets are media resources(not styles, colors, strings) resources. They refers to photos, audio, video etc used within the app.
* Assets are kept in ``res`` directory.


#### Why does the asset folder have multiple folder of similar files?
![](./5._Assets/pasted_image001.png)
Each folder inside stores the same assets but of varying quality, like resolution, bitrate etc. This is done to make the app look the same on different devices. 

*****


#### Why not compute relevant assets from a single best one?

* ``xxxhdpi`` is a higher resolution than ``hdpi``(on the left). Although it is possible for a higher res image to be displayed on a low res device, this compression may distort the image. So we provide a low resolution image.
* Having different assets is also useful because it makes the app lightweight in terms of processing. We are trading time(processing power) for space. This is very important for mobile devices, because they run on a battery.


#### Density Buckets
mdpi - medium density device
hdpi - high density device
xhdpi - extra high density device
![](./5._Assets/pasted_image.png)

#### How Android handles different resolutions?
If we use ``dp`` the actual size of the photo is the same across all devices.
![](./5._Assets/pasted_image002.png)
This is the case because Android known the screen's pixel density and calculates relevant dimensions based on that. It used this calculated information to select relevant assets.
![](./5._Assets/pasted_image003.png)
**Note**

* ``dp`` - Density-independent pixel, it is an abstract unit of length(i.e it makes things look the same on different devices).
* ``dpi`` - dots per inch, it is a measure of density of dots in printed media.
* ``ppi`` - pixels per inch, it is a measure of density of dots for digital graphic media.
* In Android jargon, ``dpi`` is used in place ``ppi``, which is a misnomer.


#### Why different resolutions exist?
Different resolution exist due to developments in display technology and a better lifetime of devices, making backwards compatibility a necessity.

#### How are assets kept?

* All the different folders are pasted into the ``/res`` directory. 
* Assets are not grouped by content. They are grouped only by filetype and quality.

![](./5._Assets/pasted_image004.png)

