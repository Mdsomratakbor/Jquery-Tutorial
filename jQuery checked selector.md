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
