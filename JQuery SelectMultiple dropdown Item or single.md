# jQuery selected selector

## What is jQuery selected selector?
`The :selected selector selects option elements that are pre-selected. Note: This selector will not work on checkboxes or radio buttons. Use the :checked selector instead.`
## How to get selected option from single select dropdown in jquery?
`<html></br>
<head></br>
    <title></title></br>
    <script src="jquery-1.11.2.js"></script></br>
    <script type="text/javascript"></br>
        $(document).ready(function () {</br>
            $('#selectCountries').change(function () {</br>
                var selectedOption = $('#selectCountries option:selected');</br>
                $('#divResult').html('Value = ' + selectedOption.val()</br>
                    + ', Text = ' + selectedOption.text());</br>
            });</br>
        });</br>
    </script></br>
</head></br>
<body style="font-family:Arial"></br>
    Country:</br>
    <select id="selectCountries"></br>
        <option selected="selected" value="USA">United States</option></br>
        <option value="IND">India</option></br>
        <option value="UK">United Kingdom</option></br>
        <option value="CA">Canada</option></br>
        <option value="AU">Australia</option></br>
    </select></br>
    <br /><br />
    <div id="divResult"></div></br>
</body></br>
</html></br>`
