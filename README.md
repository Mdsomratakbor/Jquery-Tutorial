# What is Jquery?
jQuery is a lightweight, "write less, do more", JavaScript library.
The purpose of jQuery is to make it much easier to use JavaScript on your website.

jQuery takes a lot of common tasks that require many lines of JavaScript code to accomplish, and wraps them into methods that you can call with a single line of code.

jQuery also simplifies a lot of the complicated things from JavaScript, like AJAX calls and DOM manipulation.

The jQuery library contains the following features:

- HTML/DOM manipulation
- CSS manipulation
- HTML event methods
- Effects and animations
- AJAX
- Utilities
# Why should we use jQuery Or Advantages of using jQuery over raw JavaScript?
- JQuery is cross-browser
- jQuery is a lot more easy to use than raw javascript
- JQuery is extensible
- jQuery simplifies and has rich AJAX support
- jQuery has large development community and many plugins. Example autocomplete, textbox plugin
- Excellent documentation
# How to use jQuery i a web application?
Download the jQuery file from [jQuery.com](https://jquery.com/) and reference it in your application just like any other Javascript file.
# What is difference between jQuery 1.x and 2.x?
If you want to support IE6/7/8, then use jQuery 1.x where as if you don't have the need to support IE6/7/8 then use jQuery 2.x jQuery2.x is smaller in size than jQuery 1.x
## jQuery Syntax --- like this
**Basic Syntax : $(selector).action()**
## The Document Ready Event

### Points to remember :
1. ready() function ensures that the DOM is fully loaded.
2. $ is shortcut for jQuery.
3. All Three of the following syntaxes are equivalent:
- $(document).ready(hadler)
- $().ready(handler)(this is not recommended)
- $(handler)

 `<div class="container"></br>
      <script></br>
      $(document).ready(function(){</br>
          $('#btn-1').click(function(){</br>
            alert('jquery tutorial');</br>
          })</br>
      })</br>
      </script></br>
        <button class="btn btn-info" id='btn-1'>Part-1</button></br>
    </div></br>`
    
    
### What is $(document).ready(function()) in jquery and when to use it
    
`$(document)ready is a jQuery event. It fires as soon as the DOM is loaded and ready to be manipulated by script. this the earliest point in the page load process where the script can safety access elements in the page's html dom. This event is fired before all the images, css etc.. are fully loaded.`

### What difference between $(document).ready(function()) and $(window).loade(function) event in jquery ?
`$(window).load event fires when the DOM and all the content on the page(images, css etc) is fully loaded. Since the window load event waits for images, css etc to be fully loaded, this event fires after ready event. on the other hand $(document).ready(function()) event is fired before all the images, css etc-- are fully loaded`
### Example :-














