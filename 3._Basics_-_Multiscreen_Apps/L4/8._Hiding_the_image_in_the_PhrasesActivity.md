# 8. Hiding the image in the PhrasesActivity
Created Tuesday 05 January 2021

Our ``list_item.xml`` has an ImageView. This is a problem in PhrasesActivity where ``Word`` has no image. 

What should we do, set it to ``null``? - This will give cause the app to stop abruptly.

It would be better if we could get rid of the ImageView in case of null. This is done via the ``visibility`` attribute, it has 3 values, which are all integers:

1. ``View.VISIBLE`` - view renders as normal. This is the default visibility.

![](./8._Hiding_the_image_in_the_PhrasesActivity/pasted_image.png)

2. ``View.INVISIBLE`` - view is invisible, but still takes up space.

![](./8._Hiding_the_image_in_the_PhrasesActivity/pasted_image001.png)

3. ``VIew.GONE`` - view is completely removed. Takes up no space.

![](./8._Hiding_the_image_in_the_PhrasesActivity/pasted_image002.png)
We'll be setting the ``visibility`` to ``View.GONE`` by coding this in Java:
	content_imageView.setVisibility(View.GONE);

