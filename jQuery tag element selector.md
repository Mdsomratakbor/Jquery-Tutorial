# Tag Name selector 
- To select the elements by tag name use jQuery Element Selector Syntax:  **$(element)**
### Example :
`$('td') // Selects all td elements `
`$('div a') // Select all anchor elements that are descendants of div elements`
`$('div, span, a') // Selects all div, span and anchor elements`
### Alert the total count of td elements on the page
`<script></br>
$(document).ready(function(){</br>
 alert($('td').length)</br>
})</br>
</script>`
### Select all the tr elements on the page and changes their background color to red
`<script></br>
$(document).ready(function(){</br>
$('tc').css('background-color','red');</br>
})</br>
</script>`
