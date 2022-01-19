# 13. How to setup an event listener
Created Monday 23 November 2020

Follow these steps:

1. Define the event listener and it's behavior. Use any of the two ways we've seen before.

![](./13._How_to_setup_an_event_listener/pasted_image.png)

2. Create the reference object using its constructor.

![](./13._How_to_setup_an_event_listener/pasted_image001.png)

3. Attach the clickListener. This is done by passing the reference object to the setOnClickListener

![](./13._How_to_setup_an_event_listener/pasted_image002.png)

*****


* There's a better way(a one liner), where we don't need to create another class. We can make an anonymous class implementing View.onClickListener

![](./13._How_to_setup_an_event_listener/pasted_image003.png)

