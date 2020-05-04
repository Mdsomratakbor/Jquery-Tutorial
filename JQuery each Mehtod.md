# Jquery each() Method
### What  is Jquery each() Method?
`Jquery each() method is used to iterate over the items in a collection. For each item in a collection the anonymous function is called.The index of the element and the element itself are passed to the anonymous function.`
**Example :**
   <script></br>
        $(document).ready(function(){</br>
            $("#bookName").click(function(){</br>
                $("li").each(function(index, Element){</br>
                    alert("Index :"+index+", Element :"+$(this).text());</br>
                    if($(this).text()=='Bangla Book'){</br>
                        confirm("this is my book");</br>
                    }</br>
                })</br>
            })</br>
        })</br>
    </script></br>
    
