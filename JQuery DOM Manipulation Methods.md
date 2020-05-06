# JQuery DOM Manipulation Methods
### addClass() DOM Manipulation Method?
`One or more space-separated classes to be added to the class attribute of each matched element.`</br>
**Syntax :**` addClass("className") or addClass("className1 className2")`</br>
### removeClass() DOM Manipulation Method?
`One or more space-separated classes to be removed from the class attribute of each matched element.`</br>
**Syntax :**` removeClass("className") or removeClass("className1 className2")`</br>
### hasClass() DOM Manipulation Method?
`The hasClass() mehtod will return boolean, if the class is assigned to an elment then return true else return false`</br>
**Syntax :**` hasClass("className") or hasClass("className1 className2")`</br>
### toggleClass() Dom Manipulation Method?
`The toggleClass() method toggles between adding and removing one or more class names from the selected elements. This method checks each element for the specified class names. The class names are added if missing, and removed if already set - This creates a toggle effect`</br>
**Syntax :**` toggleClass("className") or toggleClass("className1 className2")`</br>
### wrap() Dom Manipulation Method?
`A selector, element, HTML string, or jQuery object specifying the structure to wrap around the matched elements. When you pass a jQuery collection containing more than one element, or a selector matching more than one element, the first element will be used.`</br>
**Syntax :**` wrap('<div class="className"></div>')`</br>



**Exaple :**</br>     
   <script></br>
        $(document).ready(function(){</br>
            $("#addClass").click(function(){</br>
            // $("p").removeClass("remove-class").removeAttr("style").addClass("add-class").animate({ width: "100%" }).animate({ fontSize: "46px" }).animate({ borderWidth: "30px" }).slideUp(1000).slideDown(1000);</br>
            $("p").last().removeClass("remove-class").removeAttr("style").addClass("add-class").animate({ width: "100%" }).animate({ fontSize: "46px" }).animate({ borderWidth: "30px" }).slideUp(1000).slideDown(1000).css("background","#ffff");</br>
            })</br>
            $("#removeClass").click(function(){</br>
                if($("p").last().hasClass("add-class")==true){</br>
                      $("p").last().removeClass("add-class").removeAttr("style").addClass("remove-class").animate({ width: "100%" }).animate({ fontSize: "46px" }).animate({ borderWidth: "30px" }).slideUp(1000).slideDown(1000);</br>
                }</br>    
            })</br>
            $("#toggleClass").click(function(){</br>
                $("p").first().toggleClass("remove-class add-class").fadeIn(1000).fadeOut(1000).animate({ width: "100%" }).animate({ fontSize: "46px" }).animate({ borderWidth: "30px" }).slideUp(1000).slideDown(1000);</br>
            })</br>
        })</br>
          $("#wrap").click(function(){</br>
                $("#firstP").wrap('<div class="loader"></div>').fadeIn(1000).fadeOut(1000)</br>
            })
            $("#unwrap").click(function(){</br>
                $("p").unwrap();</br>
            })</br>
            $("#warpAll").click(function () {</br>
            $("p").wrapAll().wrap('<div class="loader"></div>').fadeIn(5000).fadeOut(1000);</br>
            })</br>
            $("#wrapInner").click(function () {</br>
                $("p").wrapInner().wrap('<div class="loader"></div>').fadeIn(5000).fadeOut(1000);</br>
            })</br>
    </script></br>
