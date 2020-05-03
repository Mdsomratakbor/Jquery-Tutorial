 # jQuery Attribute Selector
 ### Syntax :
 $('[attribute]')</br>
 $('[attribute="value"]')
 
 ### Example:
 $('[title]') // Selects all elements that have titile attribute </br>
 $('div[title]') // Selects all div elements that have titile attribute </br>
 $('[title="divTitle"]') // Selects all elements that have title attribute value - divTitle </br>
 $('div[title="divTitle"]') // Selects all div elments that have title attribute value - divTitle</br>
 $('[title != "divTitle"]') // Selects all attribute that have title attribute value not equal - divTitle </br>
 or 
 $('[title:not("dive")]') // Selects all attribute that have title attribute value not equal - divTitle </br>
 $('[title *="Title"]') // Selects all attribute that have title attribute value containt - Title</br>
 $('[title ~='Title']') // Selects all elements that have title attribute value containing the given word - Title, delimited by spaces</br>
 $('[title |=myTitle]') // Selects all elements that have title attribute value equal to myTitle or starting with myTitle followed by a hyphen (-)</br>
$('[title^="div"]') // Selects all elements that have title attribute value starting with div</br>
$('[title$="Heading"]') //Selects all elements that have title attribute value ending with Heading

### How to write jQuery case-sensitive attribute selector?
   $('div[title]').filter(function(){</br>
            return $(this).attr('title').toLowerCase() == 'divtitle';</br>
          }).css('border','1px solid black');</br>
- This Example filter Method is used to all the elements that do not match the selected criteria and those matches will be returned. Parameters: criteria : It specifies a selector expression, a jQuery object or one or more elements to be returned from a group of selected elements.



 

 
 
 
