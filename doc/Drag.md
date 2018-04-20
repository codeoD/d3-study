d3.drag()
Creates a new drag behavior. The returned behavior, drag, is both an object and a function, 
and is typically applied to selected elements via selection.call.
drag(selection) 
Applies this drag behavior to the specified selection.
This function is typically not invoked directly, and is instead invoked via selection.call. 

 drag.container([container]) 
 
 drag.filter([filter])
 
 drag.touchable([touchable])
 
 drag.subject([subject])
 The returned subject should be an object that exposes x and y properties, 
 so that the relative position of the subject and the pointer can be preserved during the drag gesture. 
 
 drag.clickDistance([distance])
 
 drag.on(typenames, [listener])
 
 d3.dragDisable(window)
 
 d3.dragEnable(window[, noclick])
 
 Drag Events
target - the associated drag behavior.
type - the string “start”, “drag” or “end”; see drag.on.
subject - the drag subject, defined by drag.subject.
x - the new x-coordinate of the subject; see drag.container.
y - the new y-coordinate of the subject; see drag.container.
dx - the change in x-coordinate since the previous drag event.
dy - the change in y-coordinate since the previous drag event.
identifier - the string “mouse”, or a numeric touch identifier.
active - the number of currently active drag gestures (on start and end, not including this one).
sourceEvent - the underlying input event, such as mousemove or touchmove.
 ……
 event.on(typenames, [listener])
