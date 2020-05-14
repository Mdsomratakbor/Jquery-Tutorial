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
    
<b style="font-family: Arial, Helvetica, sans-serif;">In the following example, several calls to animate() method are chained together. By default these calls are placed into a queue to be executed one after the other in series rather than executing all of them simultaneously in parallel.</b>

 $('img').on('click',function(){</br>
                $(this)</br>
                .animate({'left':700})</br>
                .animate({'top':300})</br>
                .animate({'left':10})</br>
                .animate({'top':10})</br>
            })</br>
            
<b style="font-family: Arial, Helvetica, sans-serif;"><b>Please note:</b> By default, all HTML elements have a static position, and cannot be moved. To modify the position , set the CSS position property of the element to fixed, absolute or relative.</b>

### What is animation Queue?

`When several calls to animate() method are chained together. By default these calls are placed into a queue to be executed one after the other in series rather than executing all of them simultaneously in parallel. The name of this queue is fx.
Each HTML element has its own queue. With the following code there will be 5 calls to animate method placed in the queue of each div element. This means both div elements (myDiv1 & myDiv2) may start to execute the first call to animate method more or less at the same time. However, from the given queue the queued methods are executed one after the other in series.`

**Example :**
    $('#animateQueue').click(function () {</br>
                $('#myDiv1')</br>
                    .animate({ 'width': 500 }, 1500)</br>
                    .animate({ 'padding': 20 }, 1500)</br>
                    .animate({ 'font-size': 50 }, 1500)</br>
                    .animate({ 'border-width': 10 }, 1500)</br>
                    .animate({ 'opacity': 1 }, 1500);</br>
                $('#myDiv2')</br>
                    .animate({ 'width': 500 }, 1500)</br>
                    .animate({ 'padding': 20 }, 1500)</br>
                    .animate({ 'font-size': 50 }, 1500)</br>
                    .animate({ 'border-width': 10 }, 1500)</br>
                    .animate({ 'opacity': 1 }, 1500);</br>
            });</br>

