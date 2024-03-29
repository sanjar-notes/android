# zConclusion
Created Sunday 25 October 2020


* LinearLayout does not allow overlapping views.
* RelativeLayout does not allow weights, but it does allow overlap.



* All attributes which set the outsides of a view(i.e don't affect content) start with ``layout_``.
* Orientation must be specified for a LinearLayout.
* alignRight and layout_alignParentRight are two different things.
* The root view covers the whole screen only if both width and height are set to ``match_parent``.
* For attribute names, spaces are replaced by underscores and hypenated words are written in camelcase.
* Attribute names are actually a type of active voice. This quells ambiguity. e.g ``layout_toRightOf`` is better than ``layout_right`` which is ambiguous.
* 0dp for weighted children in LinearLayout improves readability.
* Prefer LinearLayout over RelativeLayout unless necessary, KISS.
* All ``id``s, and resource references are simply integers in Java. They are not a special class or data type.


*****


* Reuse code - helps in updates, decreases impact of change etc.
* Start from figuring out the data and logic, then design the app UI.
* Steps for UI design:
	1. Decide the views
	2. Position the views
	3. Style the views
* Get news from the Android Dev Blog.
* Read things, and what they do. If it is required, see how it's done.
* Not all elements in Android end with view, e.g Button.


