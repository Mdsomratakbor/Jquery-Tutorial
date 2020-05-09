# JQuery change() Event 
`The change event is sent to an element when its value changes. This event is limited to <input> elements, <textarea> boxes and <select> elements. For select boxes, checkboxes, and radio buttons, the event is fired immediately when the user makes a selection with the mouse, but for the other element types the event is deferred until the element loses focus.`
**<script>
        $(document).ready(function(){
            var result= '';
            $("input").change(function(){
                if(result==""){
                    result = $(this).val();
                }
                else{
                    result += ", " + $(this).val();
                }               
                 $("#result").html(result);
            })
            $("#ddlCity").change(function(){
                result = $(this).val();
                if(result=='Select'){
                    alert("Please select cith");
                     $("#divResult").empty();
                }
                else{
                    $("#divResult").html(result);
                }               
            })         
           $("img").mouseover(function(){
               $("#"+ GetDivId(this)).fadeIn(500)
               $("img").css("cursor","pointer")
           }).mouseout(function(){
                $("#" + GetDivId(this)).fadeOut(500)
           })
           function GetDivId(helpIconId){
                 helpIconId = $(helpIconId).attr("id"); 
                return helpIconId.replace("img", "div")
           }
        })
    </script>**
