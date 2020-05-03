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
## How to get all selected options from multi-select dropdown in jquery?
`<!DOCTYPE html></br>
<html lang="en"></br>
<head></br>
    <meta charset="UTF-8"></br>
    <meta name="viewport" content="width=device-width, initial-scale=1.0"></br>
    <title>Drop Down item multiple or single select</title></br>
    <link rel="stylesheet" href="css/bootstrap.css" /></br>
    <link rel="stylesheet" href="fontawesome-free-5.12.1-web/css/fontawesome.css" /></br>
    <script type="text/javascript" src='js/jquery.min.js'></script></br>
    <script type="text/javascript" src='js/bootstrap.min.js'></script></br>
</head></br>
<body style="font-family:Arial"></br>
    <div class="container"></br>
        <h2>DropDown item multiple or single select</h2></br>
        <hr></br>
<div class="form-group"></br>
    <label>Country</label></br>
    <select id="selectCountries" class="form-control" multiple="multiple"></br>
        <option selected="selected" value="USA">United States</option></br>
        <option value="IND">India</option></br>
        <option value="UK">United Kingdom</option></br>
        <option value="CA">Canada</option></br>
        <option value="AU">Australia</option></br>
    </select></br>
</div></br>
    <br />
    <div id="divResult"></div></br>
    </div></br>
    <script></br>
        $(document).ready(function(){</br>
            $("#selectCountries").change(function(){</br>
                var selectCountries =  $("#selectCountries option:selected");</br>
                var resultString = "";</br>
                if(selectCountries.length>0){</br>
                    selectCountries.each(function(){ </br>                       
                        resultString += "Value = "+$(this).val()+", Text = "+$(this).text()+'</br>';</br>
                    })</br>
                }</br>
                $("#divResult").html(resultString);</br>
            })</br>
        })</br>
    </script></br>
</body></br>
</html></br>`
