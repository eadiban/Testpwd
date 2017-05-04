# Testpwd
<html>
<body>
<head>
<title>Password</title>
<script>
function checkPass(){
  var guess = document.myForm.pwdGuess.value;
  var secret = document.myForm.hdnSecret.value;
  if (guess == secret){
    document.myForm.txtOutput.value = "You may proceed.";
  } else {
    document.myForm.txtOutput.value = "That is incorrect.";
  }
}
</script>
</head>
<body>
<center>
<h1>Password<hr></h1>
<form name = "myForm">
<table>
<tr>
  <td>Please enter password</td>
  <td><input type = "password"
             name = "pwdGuess">
</tr>

<tr>
  <td colspan = 2><center>
    <input type = "button"
           value = "click me"
           onClick = "checkPass()"></center>
  </td>
</tr>

<tr>
  <td colspan = 2>
    <center>
    <textArea name = "txtOutput"
              rows = 1
              cols = 35>
    </textarea>
    </center>
  </td>
</tr>
</table>
<input type = "hidden"
       name = "hdnSecret"
       value = "JavaScript">
</form>
<hr>

</center>
</body>
</html>
</body>
