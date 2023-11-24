<!DOCTYPE html>
<html>
    <head>
        <title>
            validation
        </title>
    </head>
    <body>
        <script>
            function validatform(){
            var name=document.myform.name.value;
            var password =document.myform.password.value;
            if(name==null|| name=="")
            {
                alert("Name can't ba blank");
                return false;

            }
            else if(password.length <=6)
            {
                alert("please enter the valid password");
                return false;
            }
        }
        </script>
        <form name="myform" method="post" action="copypath" onsubmit="return validatform()">
            name:<input type="text" name="name"><br/>
            password:<input type="password" name="password"><br/>
            <input type="submit" value="click">
        </form>
    </body>
</html>
  
  
