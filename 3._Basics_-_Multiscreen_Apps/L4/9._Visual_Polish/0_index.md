# 9. Visual Polish
Created Tuesday 05 January 2021

While making the app functional, we should mostly ignore visual elements. But after the app works as accepted, we must add visual polish to the app before releasing the app.

#### Red Lines
The designer gives us the screens with red lines drawn on them. This is like a very simple engineering drawing. All dimensions are exact.
[Here's](./9._Visual_Polish/miwok-redlines.pdf) one redline document.
![](./9._Visual_Polish/pasted_image.png)
We have a different background color for each section.
For now let us set the background to orange, we'll change it later.

#### Layout Bounds
It is helpful if we could look at the bounds while the app is running, and not just in the XML viewer. Android supports this.

* Enable *Developer Options > Show layout bounds. *It can be disabled later on, this is just for developers.

The screen will look something like this:
![](./9._Visual_Polish/pasted_image002.png)

#### Doing it - mentioning only new stuff
In list_item.xml

1. Set background to a light 
2. Set background of the LinearLayout containing text to a dark color.
3. Divide the text height equally.
4. Use ``gravity`` to ``bottom`` and ``top`` for the ``TextView`` on the top and bottom.


* We learn that background is applied to everything inside the Viewgroup.


