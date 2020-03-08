## jQuery Id selector
- jQuery #id selectors uses the JavaScript document.getElementById() function

- jQuery #id selector is the most efficient among all jQuery selectors. If you konw the id of an element that you want to find, then always use the id selectors
- HTML element IDs must be unique on the page. jQuery id selector returns only the first element, if you have 2 or more elements with the same ID.

- Java Script's document.getElementById() function throws an error if the element with the given id is not fount, where as jQuery id selector will not thrown an error. To check if element is returned by #id selectors use length property.

- JavaScript's document.getElementById() and jQuery(#id) slector are not the same.
document.getElementById() returns a raw DOM object where as jQuery('#id') selector returns a jQuery object that wraps the DOM object and provides jQuery methods. This is the reason you are able to call jQuery methods like css(),click(),mouseover() on the object returned by jQuery. To get the underlying DOM object from a jQuery object use $('#id')[0]

- document.getElementById() is faster than jQuery id selector. Use document.getElementById() and $('#id') selectors unless you need the extra functionality provided by the jQuery object
