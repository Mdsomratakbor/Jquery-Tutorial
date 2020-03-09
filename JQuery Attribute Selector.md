 #jQuery Attribute Selector
 ### Syntax :
 $('[attribute]')</br>
 $('[attribute="value"]')
 
 ### Example:
 $('[title]') // Selects all elements that have titile attribute </br>
 $('div[title]') // Selects all div elements that have titile attribute </br>
 $('[title="divTitle"]') // Select all elements that have title attribute value - divTitle </br>
 $('div[title="divTitle"]') // Select all div elments that have title attribute value - divTitle</br>
 $('[title != "divTitle"]') // Select all attribute that have title attribute value not equal - divTitle </br>
 or 
 $('[title:not("dive")]') // Select all attribute that have title attribute value not equal - divTitle </br>
 $('[title *="Title"]') // Select all attribute that have title attribute value containt - Title</br>
 
