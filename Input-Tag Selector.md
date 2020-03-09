### What difference between $('intput') and $(':input') tag element selector?
$(':input') selector select all input elements like input, textarea, select and button </br>
where as $('input') selector select just input elments 
- jQuery code to get textbox value using $('input')
<script></br>
$(document).ready(function(){</br>
$('input').each(function () {</br>
   alert($(this).val())</br>
  })</br>
})</br>
</script></br>
- jQuery code to get textbox value using $(':input')
<script></br>
$(document).ready(function(){</br>
$(':input').each(function () {</br>
   alert($(this).val())</br>
  })</br>
})</br>
</script></br>

### Which one is better for performance $('input[type="text"]') or $(':input[type="text"]')
$('input[type="text"]') is better for performance over $(':input[type="text"]').</br> 
This is because $(':input[type="text"]') needs to scan all input elements, textarea,</br> select etc, where as $('input[type="text"]') scans only input elements.</br>
So if you want to find elements with an input tag, it is always better to use </br>$('input[type="text"]') over $(':input[type="text"]')
