### How to Using Jquery show password in html password field?

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
