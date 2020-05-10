# jQuery how to check if event is already bound

### Why is it important to check if an event is already bound?
`To prevent attaching event handler multiple times`
`The following example checks if a click event handler is already bound. If it's not already bound, then a click event handler is attached.`

 <script type="text/javascript"></br>
        $(document).ready(function () {</br>
            var jQueryObject = $('#btn');</br>
            var rawDOMElement = jQueryObject.get(0);</br>
            var eventObject = $._data(rawDOMElement, 'events');</br>
            if (eventObject != undefined && eventObject.click != undefined) {</br>
                alert('Click event exists');</br>
            }</br>
            else {</br>
                $('#btn').on('click', function () {</br>
                    alert('Button Clicked');</br>
                });</br>
            }</br>
        });</br>
    </script>

**Please note that this only works if you have attached event handlers using jQuery. This will not work if you have attached event handlers using raw JavaScript or element attributes.**

`Another way to prevent attaching event handlers multiple times is by using jQuery off() and on() methods. The off() method ensures that all existing click event handlers of the button are removed before again adding a new click event handler using on() method.`

$('#btn').off('click').on('click', function () {</br>
    alert('Button Clicked');</br>
});</br>
