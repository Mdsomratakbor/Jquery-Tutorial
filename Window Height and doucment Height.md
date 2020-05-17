# Window Height and Document Height 

### What is the difference between window height and document height?
`The window height is what you see (i.e browser viewport), but the document height includes everything below or above the visible area.`
<table border="1" style="border-collapse: collapse;">
<tbody>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;"><b>$(window).height()
</b></span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">Returns height of the browser window i.e browser viewport
</span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;"><b>$(document).height()
</b></span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">Returns height of HTML document
</span></td>
</tr>
<tr>
<td><span style="font-family: Arial, Helvetica, sans-serif;"><b>$(window).scrollTop()
</b></span></td>
<td><span style="font-family: Arial, Helvetica, sans-serif;">Returns the current vertical position of the scroll bar</span></td></tr>
</tbody></table>

### How to detect if the user has scrolled to the bottom of the page?
`Here is the formula to detect if the user has scrolled to the bottom of the page`

**if (verticalScrollBarPosition == $(document).height() - $(window).height()) {
    floatingDiv.html('Reached the bottom of the page');
}**

### Why window height and document height are the same in Google chrome

`Without DOCTYPE tag Chrome reports the same value for both window height and document height. Include the following DOCTYPE
declaration <!DOCTYPE html>`
