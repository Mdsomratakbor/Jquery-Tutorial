# What is AJAX ?
`AJAX stands for Asynchronous JavaScript and XML. AJAX is a new technique for creating better, faster, and more interactive web applications with the help of XML, HTML, CSS, and Java Script.`

<ul class="list">
<li><p>Ajax uses XHTML for content, CSS for presentation, along with Document Object Model and JavaScript for dynamic content display.</p></li>
<li><p>Conventional web applications transmit information to and from the sever using synchronous requests. It means you fill out a form, hit submit, and get directed to a new page with new information from the server.</p></li>
<li><p>With AJAX, when you hit submit, JavaScript will make a request to the server, interpret the results, and update the current screen. In the purest sense, the user would never know that anything was even transmitted to the server.</p></li>
<li><p>XML is commonly used as the format for receiving server data, although any format, including plain text, can be used.</p></li>
<li><p>AJAX is a web browser technology independent of web server software.</p></li>
<li><p>A user can continue to use the application while the client program requests information from the server in the background.</p></li>
<li><p>Intuitive and natural user interaction. Clicking is not required, mouse movement is a sufficient event trigger.</p></li>
<li><p>Data-driven as opposed to page-driven.</p></li>
</ul>

### Rich Internet Application Technology

<p>AJAX is the most viable Rich Internet Application (RIA) technology so far. It is getting tremendous industry momentum and several tool kit and frameworks are emerging. But at the same time, AJAX has browser incompatibility and it is supported by JavaScript, which is hard to maintain and debug.</p>

### AJAX is Based on Open Standards
**AJAX is based on the following open standards −**
<ul class="list">
<li>Browser-based presentation using HTML and Cascading Style Sheets (CSS).</li>
<li>Data is stored in XML format and fetched from the server.</li>
<li>Behind-the-scenes data fetches using XMLHttpRequest objects in the browser.</li>
<li>JavaScript to make everything happen.</li>
</ul>

**Syntax :**
<span style="font-family: Arial, Helvetica, sans-serif;">load( url [, data ] [, complete ] )</span>
<table border="1" style="border-collapse: collapse;">
    <tbody>
<tr style="background-color: #ffc000;">
        <td><span style="font-family: Arial, Helvetica, sans-serif;"><b>Parameter
        </b></span></td>
        <td><span style="font-family: Arial, Helvetica, sans-serif;"><b>Description
        </b></span></td>
    </tr>
<tr>
        <td><span style="font-family: Arial, Helvetica, sans-serif;">url
        </span></td>
        <td><span style="font-family: Arial, Helvetica, sans-serif;">Required. URL to which the request is sent
        </span></td>
    </tr>
<tr>
        <td><span style="font-family: Arial, Helvetica, sans-serif;">data
        </span></td>
        <td><span style="font-family: Arial, Helvetica, sans-serif;">Optional. A JSON object or string that is sent to the server along with the request
        </span></td>
    </tr>
<tr>
        <td><span style="font-family: Arial, Helvetica, sans-serif;">complete
        </span></td>
        <td><span style="font-family: Arial, Helvetica, sans-serif;">A callback function that is called when the request completes
        </span></td>
    </tr>
</tbody></table>
`The following example loads HTML data from the server. When a text box receives focus, the help text&nbsp;associated&nbsp;with that&nbsp;`</br>
`When the focus is lost the help text disappears.`
