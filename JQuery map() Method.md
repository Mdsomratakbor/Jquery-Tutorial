# JQuery map() Method 
### What is JQuery map() Method?
`Just like jquery each() method, map() method is also used to iterate over matched elements. `</br>
`
In general, if you want to create an array or concatenated string based on all matched elements in a jQuery selector, it is better to use map() over each() method.`</br>

**Consider the following HTML**
<ul>
    <li>US</li>
    <li>India</li>
    <li>UK</li>
    <li>Canada</li>
    <li>Australia</li>
</ul>

**Using each() method**</br>
$(document).ready(function () {</br>
var data =""</br>
     $("#each").click(function(){</br>
                $("li").each(function(index,element){</br>
                    data+="Text : "+ $(this).text()+" |";</br>
                })</br>
                data = data.substr(0, data.length-1);</br>
                $("#result").html(data);</br>
            })</br>
});</br>

**Using map() method**</br>
$(document).ready(function () {</br>
     var data = "";</br>
            $("#each").click(function(){</br>
               data= $("li").map(function(index, element){</br>
                    return $(this).text();</br>
                }).get().join(" | ")</br>
                 $("#result").html(data);</br>
            })</br>
});</br>

### What difference between $.each() and $.map() method in jquery?
<table border="1" style="border-collapse: collapse;">
<tbody>
<tr>
<td style="background-color: #e46c0a;"><span style="font-family: Arial, Helvetica, sans-serif;"><b>$.map
</b></span></td>
<td style="background-color: #e46c0a;"><span style="font-family: Arial, Helvetica, sans-serif;"><b>$.each
</b></span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;">map method can be used as an iterator.
</span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">each method is an immutable iterator
</span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;">Returns a new array
</span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">Returns the original array
</span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;">The order of callback arguments - element, index.</span><br>
<span style="font-family: Arial, Helvetica, sans-serif;">$.map(elems, <span style="color: blue;">function </span>() { element, index }, arg)
</span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">The order of callback arguments - index, element.</span><br>
<span style="font-family: Arial, Helvetica, sans-serif;">$.each(elems, <span style="color: blue;">function </span>() { index, element }, arg)
</span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;">Does not have a way to terminate the iteration
</span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">Return false to terminate the iteration
</span></td>
</tr>
</tbody></table>
<span style="font-family: Arial, Helvetica, sans-serif;"><b>Example :</b> Notice that the callback arguments in the each method are the reverse of the callback arguments in the map function. Also notice that map returns a new array where as each method returns the original array. This proves the point that each method is an immutable iterator where as map is not.</span></br
 var intArray = [1,2,2,3,2,5,5,2,85,656,56,56,56,265,9,62,629,26,2,562,6]
            $("#each").click(function(){
                function functionA(index,element){
                    return element*5;
                }
                function functionB(element, index){
                    return element*5;
                }
                document.write($.each(intArray, functionA)+"</br>");
                document.write($.map(intArray, functionB));
                
            })
