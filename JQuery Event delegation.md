# JQuery event delegation

### What is event delegation?
`Event delegation allows us to attach a single event listener, to a parent element, that will fire for all descendants matching a selector, whether those descendants exist now or are added in the future. Both on() and delegate() functions allow us to perform event delegation.`

**Syntax : **`$( document ).delegate( selector, events, data, handler );  // jQuery 1.4.3+`</br>
`$( document ).on( events, selector, data, handler ); `</br>

**How does the following example work :** 

1. When you click on a list item (li), the event gets bubbled up to its parent (ul) as the list item (li) does not have it's own click event handler 
2. The bubbled event is handled by the the parent (ul) element, as it has a click event handler.
3. When a new list item is added dynamicaly, you don't have to add the click event handler explicitly to it. Since the newly created list item (li) is added to the same parent element (ul), the click event of this list item also gets bubbled upto the same parent and will be handled by it.
4. undelegate() stops event delegation

<img alt="jQuery delegate function" border="1" src="http://1.bp.blogspot.com/-rg-Y_vExop0/VUPz998CvWI/AAAAAAAAa0U/BddiXhUAF7U/s1600/jQuery%2Bdelegate%2Bfunction.png">

<span style="font-family: Arial, Helvetica, sans-serif;">If you are using <b>jQuery 1.7 or higher</b> version, jQuery recommends to use <b>on()</b> to perform event delegation instead of <b>delegate()</b>. The above example can be very easily rewritten using <b>on() </b>and <b>off() </b>functions, instead of <b>delegate() </b>and <b>undelegate() </b>functions as shown below.</span>


 <script></br>
        $(document).ready(function () {</br>
           $("#btnClickMe").on("click",function(){      </br>   
               var data = "<li>Hello UK</li>";</br>
               $("ul").append(data);</br>
           })</br>
           $("ul").on("click","li",function(){</br>
               $(this).css('cursor', 'pointer').fadeOut(500);</br>
           })</br>
             $("#btnUndelegate").on("click", function () {</br>
                $("ul").off('click', 'li');</br>
            })</br>
           $("#btnClickMe").on("click", function () {</br>
                var data = "<li>Hello UK</li>";</br>
                $("ul").append(data);</br>
            })</br>
            $("ul").delegate("li", "click",  function () {</br>
                $(this).css('cursor', 'pointer').fadeOut(500);</br>
            })</br>
            $("#btnUndelegate").on("click",function(){</br>
                $("ul").undelegate('li', 'click');</br>
            })          </br>
        })</br>
    </script></br>
