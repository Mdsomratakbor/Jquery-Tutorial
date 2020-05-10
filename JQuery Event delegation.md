# JQuery event delegation

### What is event delegation?
`Event delegation allows us to attach a single event listener, to a parent element, that will fire for all descendants matching a selector, whether those descendants exist now or are added in the future. Both on() and delegate() functions allow us to perform event delegation.`

**How does the following example work :** 

1. When you click on a list item (li), the event gets bubbled up to its parent (ul) as the list item (li) does not have it's own click event handler 
2. The bubbled event is handled by the the parent (ul) element, as it has a click event handler.
3. When a new list item is added dynamicaly, you don't have to add the click event handler explicitly to it. Since the newly created list item (li) is added to the same parent element (ul), the click event of this list item also gets bubbled upto the same parent and will be handled by it.
4. undelegate() stops event delegation

<img alt="jQuery delegate function" border="1" src="http://1.bp.blogspot.com/-rg-Y_vExop0/VUPz998CvWI/AAAAAAAAa0U/BddiXhUAF7U/s1600/jQuery%2Bdelegate%2Bfunction.png">
