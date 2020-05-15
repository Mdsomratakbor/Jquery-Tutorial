# Create Floating Div Using JQuery

### How to create floating div using jQuery?

`We want the div element in the sidebar to be floating and always visible as we scroll down the page.`
<img alt="jquery floating div" src="http://1.bp.blogspot.com/-Vmcf_eGm4m8/VWTZI_tMMvI/AAAAAAAAbS0/B3fxHIaePDY/s1600/jquery%2Bfloating%2Bdiv.png">

<span style="font-family: Arial, Helvetica, sans-serif;"><b>Example :</b> In this example we are using position() and scrollTop() functions. The object returned by position() function has top and left properties, which can be used to know the current top and left positions (coordinates). We are using this function to find the top position of the div element that we want to keep floating as we scroll down. To get the current vertical position of the scroll bar, we are using scrollTop() function.&nbsp;</span>

<span style="font-family: Arial, Helvetica, sans-serif;">As we scroll and when the current vertical position of the scroll bar becomes GREATER THAN the top position of the div element, then we want the div element to <b>start floating</b>. To do this set <b>position </b>style to <b>fixed</b>. A fixed position element is positioned relative to the browser window. So as you scroll down it will be floating in the browser window.</span>

<span style="font-family: Arial, Helvetica, sans-serif;">If the current vertical position of the scroll bar becomes LESS THAN the top position of the div element, then we don't want the div element to float, so we set <b>position </b>style to <b>relative</b>. A relative position element is positioned relative to itself. So if you set <b>position </b>to <b>relative </b>and <b>top </b>to <b>0</b>, it will continue to stay where it is without floating.</span>

**Code :**
<script></br>
            $(document).ready(function () {</br>
              $(window).scroll(function(){</br>
                  var windowScroll = $(window).scrollTop();</br>
                  var floatingDivScroll = $("#floatingDiv").position().top;</br>
                  if(windowScroll>= floatingDivScroll){</br>
                      $("#floatingDiv").css({</br>
                          'position':'fixed',</br>
                          'top':5,</br>
                          'width':350</br>
                      })</br>
                  }</br>
                  else{</br>
                      $("#floatingDiv").css({</br>
                          'position': 'relative',</br>
                          'top': 0</br>
                      })</br>
                  }</br>
              })</br>
            })</br>
        </script></br>
