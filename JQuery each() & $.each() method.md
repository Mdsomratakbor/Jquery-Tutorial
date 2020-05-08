# JQuery each() and $.each() method

**In jQuery there are 2 versions of each() method**</br>
<ol>. each()</ol>
<ol>. $.each() or jQuery.each()</ol>

### What is Difference between each() and $.each() method in jquery?
`.each() method is used to iterate over the items in a jQuery object collection whereas $.each() method is used to iterate over javascript objects or arrays.`

**let's look it an example if we using .each**
<ul>
                    <li>Hello World</li>
                    <li>Hello Bangladesh</li>
                    <li>Hello UK</li>
                    <li>Hello India</li>
</ul>

**JQuery Code :**</br>
<script></br>
       $(document).ready(function(){</br>
    var result = '';</br>
            $('#each').click(function(){</br>
                $("li").each(function(index, element){</br>
                    result += "Index : "+index +", Text : "+$(this).text();</br>
                })</br>
                $("#result").html(result);</br>
            })</br>
            })</br>
  </script></br>

**Here, declaration of .each function:-**
`Here, we have a unorder list & this unorder list contains a few list items. So, looks it a jQuery ready function lets use the selector $(li) this selector is going to return as a jQuery object collection that will contain all the list item. If we want to iterate over all these list items in that jQuery object collection we will use .each function this function got two parameters callback and arguments. This callback parameter represents a function that we want to execute for each item that we are iterating over. This function has two parameters index & element. So, what is this index parameter represents this index parameter represents the index of the item that we are currently iterating over within this collection and the element parameter represents the element itself. So, lets every wants to print the index of the item and the value that is the list item value. let's create a result variable its initialize that empty string and within our jquery each function.`

**Let's look at an example if we using $.each**
`when we use $.each to iterate over javascript objects or arrays. let's create javascript array.`</br>
<script></br>
       $(document).ready(function(){</br>
  var jsArray = [100, 2000, 3000, 9000, 8000];</br>
            $('#doteach').click(function () {</br>
            $.each(jsArray, function(index, element){</br>
                    result += 'Index = ' + index + ', Value = ' + element + ';</br>
            })</br>
              $("#result").html(result);</br>
            })</br>
                        })</br>
  </script></br>
