### What is jQuery checked selector?
`The checked selector selects all checked check-boxes or radio buttons. Let us understand this with an example`
**Syntax :**
$('input[type="radio"]:checked')</br>
**Example :**
   <script type="text/javascript"></br>
        $(document).ready(function () {</br>
            $('#btnSubmit').click(function () {</br>
                var result = $('input[type="radio"]:checked');</br>
                if (result.length > 0) {</br>
                    $('#divResult').html(result.val() + " is checked");</br>
                }</br>
                else {</br>
                    $('#divResult').html("No radio button checked");</br>
                }</br>
            });</br>
        });</br>
    </script></br>
    
   **Another Example**
     <script></br>
      $(document).ready(function(){</br>
          $('#btnSubmit').click(function(){</br>
              var result = $('input[type="checkbox"]:checked');</br>
              if(result.length>0){</br>
               var resultString = result.length + " checkbox Chcked </br>";</br>
                 result.each(function () {</br>
                     resultString  += $(this).val() + "</br>"</br>
                      console.log($(this).val());</br>
                  })</br>
                  $('#divResult').html(resultString);</br>
              }</br>
              else{</br>
                  $('#divResult').html("No Checkbox chcked");</br>
              }</br>
          })</br>
      })</br>
  </script></br>
