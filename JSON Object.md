# JSON
### What is JSON ?
`JSON  stand for JavaScript Object Notation.JSON is a lightweight format for storing and transporting data. JSON is often used when data is sent from a server to a web page. JSON is "self-describing" and easy to understand.`
### What is JSON Array?
`JSON array represents ordered list of values. JSON array can store multiple values. It can store string, number, boolean or object in JSON array.`
`In JSON array, values must be separated by comma.`
`The [(square bracket)] represents JSON array.`</br>
**JSON Array of String :**
`Let's see an example of JSON arrays storing string values.`
**["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday"]**</br>
**JSON Array of Numbers :**</b>
`Let's see an example of JSON arrays storing number values.`</br>
**[12, 34, 56, 43, 95]**</br>
**JSON Array of Booleans :**</br>
`Let's see an example of JSON arrays storing boolean values.`</br>
**[true, true, false, false, true]**</br>
**JSON Array of Objects**</br>
`Let's see a simple JSON array example having 4 objects.`</br>
   **employeeData: [
            {
                    'firstName':'Md Hasan',
                    'LastName':'Khan',
                    'Age':42,
                    'Mail':'Hasan@gmail.com'
            },
            {
                'firstName': 'Md Kalam',
                'LastName': 'Khan',
                'Age': 22,
                'Mail': 'Kalam@gmail.com'
            },
            {
                    'firstName': 'Md Karim',
                    'LastName': 'Ullah',
                    'Age': 32,
                    'Mail': 'Karim@gmail.com'
            }
            ]**</br>

**JSON Multidimensional Array**</br>
**We can store array inside JSON array, it is known as array of arrays or multidimensional array.**</br>
[    
 [ "a", "b", "c" ],   
 [ "m", "n", "o" ],   
 [ "x", "y", "z" ]   
]


### How to Covert JSON Object to JSON String?
**Using JSON.stringify() method :**` The JSON.stringify() method in javascript allows us to take a JavaScript object or Array and create a JSON string out of it.`</br>
**Syntax :**` JSON.stringify(value, replacer, space) `
