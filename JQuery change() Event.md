# JQuery change() Event 
`The change event is sent to an element when its value changes. This event is limited to <input> elements, <textarea> boxes and <select> elements. For select boxes, checkboxes, and radio buttons, the event is fired immediately when the user makes a selection with the mouse, but for the other element types the event is deferred until the element loses focus.`
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
