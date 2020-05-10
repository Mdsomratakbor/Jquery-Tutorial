# .scroll()
`This method is a shortcut for .on( "scroll", handler ) in the first and second variations, and .trigger( "scroll" ) in the third.
The scroll event is sent to an element when the user scrolls to a different place in the element. It applies to window objects, but also to scrollable frames and elements with the overflow CSS property set to scroll (or auto when the element's explicit height or width is less than the height or width of its contents).
For example, consider the HTML:`
   <script></br>
        $(document).ready(function () {</br>
            var lastScroll = 0;</br>
            var scrollBottum = 0;</br>
            $('div').on('scroll',function(){</br>
                var currentScrollPosition = $(this).scrollTop();</br>
                if(currentScrollPosition> lastScroll){</br>
                    $(this).css('background','red').fadeOut(500).fadeIn(500);</br>
                }</br>
                else{</br>
                    $(this).css('background', 'black').fadeOut(500).fadeIn(500);</br>
                }</br>
                lastScroll = currentScrollPosition;</br>
                $("#result").html("currentScrollPosition : "+currentScrollPosition+", LastScrollPosition : "+lastScroll)</br>
            })</br>
        })</br>
    </script></br>
