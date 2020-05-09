# JQuery Event Object
### How to retrieve event data using event object
`Whenever an event (like click, mouseover, mouseout etc) occurs, the relevant data about that event is placed into the event object. For example, the event object contains event data like, the X and Y coordinates of the mouse pointer when the event occurred, the HTML element that fired the event, which mouse button is clicked etc.`
**Obtaining the event object is straightforward.**
`The event object is always passed to the event handler method. Let us understand this with an example. When we click the button, we want to capture the following event data`
1. Event name
2. Mouse X coordinate when the event occured
3. Mouse Y coordinate when the event occured
4. The control that raised the event
5. The HTML tag name that raised the event
