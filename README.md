# TestGlances

Glances bugs in watchOS 2

When loading this glance in the simulator, I see a never ending spinner. 

![glance spinner](http://i.imgur.com/zVBmIUr.png)

Sometimes there's an error: 

> ERROR -[SPRemoteInterface _interfaceControllerClientIDForControllerID:] clientIdentifier for interfaceControllerID: not found

I found a reference on [Stack Overflow](http://stackoverflow.com/a/31454888/2125714). The reprocucable bug seems to occur when a glance dipsplays an image.

To see the bug:

1. Run the watchOS app in the simulator.
2. Stop the simulation.
3. On the iOS simulator, open the companion Apple Watch app for iPhone.
4. Install the Glance for the TestGlances app.
5. On the watch simulator navigate to the glance by swiping up on the clock face.
