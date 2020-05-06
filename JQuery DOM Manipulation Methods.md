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
### toggleClass() DOM Manipulation Method?
`The toggleClass() method toggles between adding and removing one or more class names from the selected elements. This method checks each element for the specified class names. The class names are added if missing, and removed if already set - This creates a toggle effect`</br>
**Syntax :**` toggleClass("className") or toggleClass("className1 className2")`</br>
### wrap() DOM Manipulation Method?
`A selector, element, HTML string, or jQuery object specifying the structure to wrap around the matched elements. When you pass a jQuery collection containing more than one element, or a selector matching more than one element, the first element will be used.`</br>
**Syntax :**` $(selector).wrap('<div class="className"></div>')`</br>
### unwrap() DOM Mnipuulation Method?
`The .unwrap() method removes the element's parent and returns the unwrapped content. This is effectively the inverse of the .wrap() method. The matched elements (and their siblings, if any) replace their parents within the DOM structure.`</br>
**Syntax :**` $(selector).unwrap()`</br>
### wrapAll() DOM Manipulation Method?
`The .wrapAll() function can take any string or object that could be passed to the $() function to specify a DOM structure. This structure may be nested several levels deep, but should contain only one inmost element. The structure will be wrapped around all of the elements in the set of matched elements, as a single group.`</br>
**Syntax :**` $(selector).wrapAll('<div class="className"></div>')`</br>
### wrapInner() DOM Manipulation Method?
`The .wrapInner() function can take any string or object that could be passed to the $() factory function to specify a DOM structure. This structure may be nested several levels deep, but should contain only one inmost element. The structure will be wrapped around the content of each of the elements in the set of matched elements.`</br>
**Syntax :**` $(selector).wrapInner('<div class="className"></div>')`</br>
### append() DOM Manipulation Method?
`A function that returns an HTML string, DOM element(s), text node(s), or jQuery object to insert at the end of each element in the set of matched elements. Receives the index position of the element in the set and the old HTML value of the element as arguments. Within the function, this refers to the current element in the set.`</br>
**Syntax :**` $(selector).append("<div></<div>")`

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
