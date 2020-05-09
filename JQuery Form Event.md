# JQuery Form Events

### JQuery change() Event 
`This method is a shortcut for .on( "change", handler ) in the first two variations, and .trigger( "change" ) in the third.`</br>
`The change event is sent to an element when its value changes. This event is limited to <input> elements, <textarea> boxes and <select> elements. For select boxes, checkboxes, and radio buttons, the event is fired immediately when the user makes a selection with the mouse, but for the other element types the event is deferred until the element loses focus.`</br>

### JQuery blur() Event
`The blur event is sent to an element when it loses focus. Originally, this event was only applicable to form elements, such as <input>. In recent browsers, the domain of the event has been extended to include all element types. An element can lose focus via keyboard commands, such as the Tab key, or by mouse clicks elsewhere on the page.`
### JQuery focus() Event
<ul>
      <li>This method is a shortcut for <code>.on( "focus", handler )</code> in the first and second variations, and <code>.trigger( "focus" )</code> in the third.</li>
      <li>The <code>focus</code> event is sent to an element when it gains focus. This event is implicitly applicable to a limited set of elements, such as  form elements (<code>&lt;input&gt;</code>, <code>&lt;select&gt;</code>, etc.) and links (<code>&lt;a href&gt;</code>). In recent browser versions, the event can be extended to include all element types by explicitly setting the element's <code>tabindex</code> property. An element can gain focus via keyboard commands, such as the Tab key, or by mouse clicks on the element.</li>
      <li>Elements with focus are usually highlighted in some way by the browser, for example with a dotted line surrounding the element. The focus is used to determine which element is the first to receive keyboard-related events.</li>
    </ul>
 
 ### JQuery focusin() Event
 <ul>
<li> This method is a shortcut for .on( "focusin", handler ) in the first two variations, and .trigger( "focusin" ) in the third.</li>

<li>The focusin event is sent to an element when it, or any element inside of it, gains focus. This is distinct from the focus event in that it supports detecting the focus event on parent elements (in other words, it supports event bubbling).
This event will likely be used together with the focusout event.</li>   
</ul>

### JQuery focusout() Event</br>
`This method is a shortcut for .on( "focusout", handler ) when passed arguments, and .trigger( "focusout" ) when no arguments are passed.
The focusout event is sent to an element when it, or any element inside of it, loses focus. This is distinct from the blur event in that it supports detecting the loss of focus on descendant elements (in other words, it supports event bubbling).
This event will likely be used together with the focusin event.`

<script></br>
        $(document).ready(function(){</br>
            var result= '';</br>
            $("input").change(function(){</br>
                if(result==""){</br>
                    result = $(this).val();</br>
                }</br>
                else{</br>
                    result += ", " + $(this).val();</br>
                }              </br> 
                 $("#result").html(result);</br>
            })</br>
            $("#ddlCity").change(function(){</br>
                result = $(this).val();</br>
                if(result=='Select'){</br>
                    alert("Please select cith");</br>
                     $("#divResult").empty();</br>
                }</br>
                else{</br>
                    $("#divResult").html(result);</br>
                }  </br>             
            })         
           $("img").mouseover(function(){</br>
               $("#"+ GetDivId(this)).fadeIn(500)</br>
               $("img").css("cursor","pointer")</br>
           }).mouseout(function(){</br>
                $("#" + GetDivId(this)).fadeOut(500)</br>
           })</br>
           function GetDivId(helpIconId){</br>
                 helpIconId = $(helpIconId).attr("id"); </br>
                return helpIconId.replace("img", "div")</br>
           }</br>
        })</br>
    </script>
