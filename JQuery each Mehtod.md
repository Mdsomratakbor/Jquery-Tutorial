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
  ### How to exit from each function in jQuery?
  <script type="text/javascript"> </br>
     $("#bookName").click(function(){ </br>
                $("li").each(function(index, element){ </br>
                    if($(element).text()=="Math Book"){ </br>
                        return false; </br>
                    } </br>
                    alert("Text :"+$(element).text()); </br>
                }) </br>
            }) </br>
</script>
### What is Implicit iteration in jQuery?
` The $('li') selector returns all list item elements. Notice that we are calling the css() jquery function on the jquery collection itself. In this case, css() method implicitly iterates over each element in the entire collection.`</br>
**Example : Book lis **
<ul></br>
                <li>Bangla Book</li></br>
                <li>English Book</li></br>
                <li>Math Book</li></br>
                <li>Religion Book</li></br>
                <li>Story Book</li></br>
                <li>Play Book</li></br>
</ul></br>
<script></br>
   $(document).ready(function(){</br>
                $("li").each(function(index, Element){  </br>            
                    $(this).css('color','red');</br>
                }) </br>
             })</br>
</script>
    
