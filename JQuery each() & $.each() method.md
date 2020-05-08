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
**JQuery Code :**

<script></br>
       $(document).ready(function(){</br>
    var result = '';</br>
            $('#each').click(function(){</br>
                $("li").each(function(index, element){</br>
                    result += "Index : "+index +", Text : "+$(this).text()+"</br>";</br>
                })</br>
                $("#result").html(result);</br>
            })</br>
            })</br>
  </script>

