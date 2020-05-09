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

<img alt="convert javascript event to jquery event" border="1" src="http://4.bp.blogspot.com/-ZcyUpyokPFg/VTvkUYcqMUI/AAAAAAAAaq8/59jueEbMZUU/s1600/convert%2Bjavascript%2Bevent%2Bto%2Bjquery%2Bevent.png">
`Notice that in the example below, we are passing event object to getEventDetails() method. This object is the raw JavaScript event object. The type property gives us the event name that occured. pageX and pageY properties return the X and Y coordinates of the mouse pointer. Target property returns the HTML element that raised the event. Target, pageX and pageY properties are supported by all modern browsers and Internet Explorer 9 and above. The following code will not work in Internet Explorer 8 and earlier versions. In addition to click event, the following example returns mouseover and mouseout event data.
`
