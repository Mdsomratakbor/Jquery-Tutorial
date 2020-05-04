# jQuery method chaining
###  What is method chaining?
`The jQuery provides another robust feature called method chaining that allows us to perform multiple action on the same set of elements, all within a single line of code.
This is possible because most of the jQuery methods return a jQuery object that can be further used to call another method. Here's an example.`
<script></br>
        $(document).ready(function(){</br>
            $("#startChaining").click(function(){</br>
                $("p").animate({width:"100%"}).animate({ fontSize:"46px"}).animate({</br> borderWidth:"30px"}).slideUp(1000).slideDown(1000).css("background","#ffff")</br>
            })</br>
            $("#resetChaining").click(function(){</br>
                $("p").removeAttr("style");</br>
            })</br>
        })</br>
    </script></br>
### When will method chaining not work?
`Method chaining will not work if a method in the chain does not return an object. In the example below, text() method returns a string that contains the text of all the list items and not an object. Hence the chaining does not work in this case.Here's an example.`
<script></br>
        $(document).ready(function(){</br>
            $("#startChaining").click(function(){</br>
                $("p").text().animate({width:"100%"}).animate({ fontSize:"46px"}).animate({</br> borderWidth:"30px"}).slideUp(1000).slideDown(1000).css("background","#ffff")</br>
            })</br>
            $("#resetChaining").click(function(){</br>
                $("p").removeAttr("style");</br>
            })</br>
        })</br>
    </script></br>
    
