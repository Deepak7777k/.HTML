# .HTML
<!DOCTYPE html>
<html>
<head>
<title>Registration Page</title>
<script>
function validateForm() {
  var firstname = document.forms["regForm"]["fname"].value;
  var lastname = document.forms["regForm"]["lname"].value;
  var email = document.forms["regForm"]["email"].value;
  var phone = document.forms["regForm"]["phone"].value;
  if (firstname == "") {
    alert("Firstname must be filled out");
    return false;
  }
  if (lastname == "") {
    alert("Lastname must be filled out");
    return false;
  }
  if (email == "") {
    alert("Email must be filled out");
    return false;
  }
  if (phone == "") {
    alert("Phone must be filled out");
    return false;
  }
}
</script>
</head>
<body>
<form name="regForm" onsubmit="return validateForm()" action="registration.php" method="post">
  First Name: <input type="text" name="fname" />
  <br><br>
  Last Name: <input type="text" name="lname" />
  <br><br>
  Email: <input type="text" name="email" />
  <br><br>
  Phone No.: <input type="text" name="phone" />
  <br><br>
  <input type="submit" value="Submit" />
  <input type="reset" value="Reset" />
</form>
</body>
</html>
