# JQuery Simple Progressbar 

### First code

<script></br>
        $(document).ready(function () {</br>
            var currentPercentage = 0;</br>
            var priviousPercentage = 0;</br>
            function animateProgressbar(priviousPercentage, currentPercentage){</br>
                $("#innerDiv").animate({</br>
                    'width':(currentPercentage*500)/100</br>
                },3000)</br>
                if(priviousPercentage>currentPercentage)</br>
                currentPercentage-=1;</br>
                $({counter :priviousPercentage}).animate({ counter:currentPercentage},{</br>
                    duration:3000,</br>
                step:function(){</br>
                    $("#innerDiv").text(Math.ceil(this.counter)+" %") </br>
                }})</br>
            }</br>
            $("#myButton").click(function(){</br>
                priviousPercentage = currentPercentage;</br>
                currentPercentage = $("#ddlPercentages").val()</br>
                animateProgressbar(priviousPercentage, currentPercentage);</br>
            })</br>
        })</br>
    </script></br>
