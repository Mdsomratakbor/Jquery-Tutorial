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
