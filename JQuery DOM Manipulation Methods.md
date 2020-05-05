# JQuery DOM Manipulation Methods
### addClass() DOM Manipulation Method?
`One or more space-separated classes to be added to the class attribute of each matched element.`</br>
**Syntax :**` addClass("className") or addClass("className1 className2")`</br>
### removeClass() DOM Manipulation Method?
`One or more space-separated classes to be removed from the class attribute of each matched element.`</br>
**Syntax :**` removeClass("className") or removeClass("className1 className2")`</br>
**Exaple :**</br>     
   <script></br>
        $(document).ready(function(){</br>
            $("#addClass").click(function(){</br>
            // $("p").removeClass("remove-class").removeAttr("style").addClass("add-class").animate({ width: "100%" }).animate({ fontSize: "46px" }).animate({ borderWidth: "30px" }).slideUp(1000).slideDown(1000);</br>
            $("p").last().removeClass("remove-class").removeAttr("style").addClass("add-class").animate({ width: "100%" }).animate({ fontSize: "46px" }).animate({ borderWidth: "30px" }).slideUp(1000).slideDown(1000);</br>
            })</br>
            $("#removeClass").click(function(){</br>
                if($("p").last().hasClass("add-class")==true){</br>
                      $("p").last().removeClass("add-class").removeAttr("style").addClass("remove-class").animate({ width: "100%" }).animate({ fontSize: "46px" }).animate({ borderWidth: "30px" }).slideUp(1000).slideDown(1000);</br>
                }</br>    
            })</br>
        })</br>
    </script></br>
