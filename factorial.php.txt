<html>
<body>
<form method="post">
Enter the number<input type="text" name="t1"><br>
<input type="submit" name="submit" value="submit">
</form>
<?php
function fact($f){
  if ($f == 0) {
    return 1;
  } else {
    return $f * fact($f - 1);
  }
}

if (isset($_POST['submit'])) {
  $f = $_POST['t1'];
  echo "The factorial is:".fact($f); 
}
?>
</body>
</html>