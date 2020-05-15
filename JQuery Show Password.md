### How to Using Jquery show password in html password field?


**First Code :**

  <script></br>
            $(document).ready(function () {</br>
 $("#checkShowPassword").click(function(){</br>
                var currentPasswordFiled = $("#showPassword");</br>
                var currentPassword = currentPasswordFiled.val();</br>
                $(currentPasswordFiled).remove();</br>
                if ($("#checkShowPassword").is(":checked")) {</br>
                    $("#passwordFiled").after("<input type=text' id='showPassword' class='form-control' value='" + currentPassword + "'/>")</br>
                }</br>
                else {</br>
                    $("#passwordFiled").after('<input type="password" class="form-control" id="showPassword" value="' + currentPassword + '"/>')</br>
                }</br>
            })</br>
            })</br>
        </script></br> 
        
        
            
**Second Code :**
  <script></br>
            $(document).ready(function () {</br>
              $("#checkShowPassword").on({</br>
                  click:function(){</br>
                    $("#showPassword").attr("type",$("#checkShowPassword").is(":checked")?'text':'password')</br>
                  },</br>
                  mouseover:function(){</br>
                      if($("#showPassword").val()==null){</br>
                          alert("Please enter the password")</br>
                      }          </br>         
                  }</br>
              })</br>
            })</br>
        </script></br>
