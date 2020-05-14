# JQuery animate() function
### What is JQuery animate() funcion?
`The animate() method performs a custom animation of a set of CSS properties. This method changes an element from one state to another with CSS styles. The CSS property value is changed gradually, to create an animated effect. Only numeric values can be animated (like "margin:30px").`

**Syntax of jquery animate function :**</br>
`.animate( properties [, duration ] [, easing ] [, complete ] )`
<table border="1" style="border-collapse: collapse;">
<tbody>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;"><b>Parameter
</b></span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;"><b>Description
</b></span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;">properties
</span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">An object of CSS properties and values
</span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;">duration
</span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">The duration for animation in milliseconds. Default is 400.
</span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;">easing
</span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">Easing function to use for the transition. Default is swing. You could also use linear.
</span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;">complete
</span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">A function to call once the animation is complete
</span></td></tr>
</tbody></table>

Animate function has 4 parameters. Only the first parameter (properties) is the required parameter. Rest 3 are optional.

### What is jQuery easing?
`Easing is a technique where the speed and/or direction of animation are changed while the animation is in progress. Easing can make the animation start off slow and gradually speed up, start up fast and gradually slow down, and a whole host of other effects. The difference between linear and swing easing is very subtle.`

**The following example increases the height and width of the image to 400 pixels on mouseover. On mouseout the height and width are reduced to 100 pixels.**
<script></br>        
        $(document).ready(function () {  </br>      
            $("#animate").on('click',()=>{    </br>     
                $("p").animate({</br> 
                    height: '250px',</br> 
                    width: '300px',     </br>               
                    fontSize:'20px'</br> 
                },2000).animate({ backgroundColor: '#f5f5f5',},2000)</br> 
            })</br> 
            $('img').on({</br> 
                mouseover:function(){</br> 
                    $(this).animate({</br> 
                        height:'500px',</br> 
                        width :'500px'</br> 
                    },3000,'linear',animateComplete)</br> 
                },</br> 
                mouseout:function(){</br> 
                    $(this).animate({</br> 
                        height: '200px',</br> 
                        width: '200px'</br> 
                    },3000)</br> 
                }</br> 
            });</br> 
            function animateComplete(){</br> 
                alert("animation complete")</br> 
            }</br> 
        })</br> 
    </script></br> 


