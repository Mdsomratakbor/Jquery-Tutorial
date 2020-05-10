# JQuery one() method

### How to execute event of an element only once.?
`If you want to execute event of an elment only once time trigger, there are two way `
<ol>
  <li>Using on() and off() method </li>
  <li>Using one() method </li>
 </ol>
 
 ### How to using on() and off() method execute event of an element only once.?
 
 `Let us understand this with an example.`
 $(document).ready(function () {</br>
    $('#btn').on({</br>
        mouseover: function () {</br>
            $(this).css('background-color', 'yellow');</br>
            $(this).off('mouseover');</br>
        },</br>
        mouseout: function () {</br>
            $(this).css('background-color', 'white');</br>
            $(this).off('mouseout');</br>
        },</br>
        click: function () {</br>
            alert('Button clicked');</br>
            $(this).off('click');</br>
        }</br>
    });</br>
});</br>
  ### How to using one() method execute event of an element only once.?
 
 `Let us understand this with an example.`
 $(document).ready(function () {</br>
    $('#btn').one({</br>
        mouseover: function () {</br>
            $(this).css('background-color', 'yellow');</br>
        },</br>
        mouseout: function () {</br>
            $(this).css('background-color', 'white');</br>
        },</br>
        click: function () {</br>
            alert('Button clicked');</br>
        }</br>
    });</br>
});</br>
 
