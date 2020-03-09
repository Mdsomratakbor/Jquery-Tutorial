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
