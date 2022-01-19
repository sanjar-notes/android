# Questions
Created Monday 14 December 2020


17. Okay, only having views that are currently on screen saves a lot of memory. But 'recycling views', i.e setting new content for old views, instead of destroying them(old ones) and creating new ones doesn't contribute to saving space, aren't the two ways equivalent?
18. Correct, creating new views(and destroying old ones) or replacing content in old views is **asymptotically** equivalent(space). But 'recycling views' is done to save time, not space. We chose recycling(content replacement) because the process of inflating views(i.e creating new Java objects) from XML is a slow process, and we want to avoid it.



17. Does View Recycling have anything to do with re-rendering?
18. No, if a list is scrollable, re-rendering is inevitable. Recyling views has got nothing to do with re-rendering.


