<html>
<body>
<form method="post">
Enter the limit: <input type="text" name="t1"><br>
<input type="submit" name="submit" value="submit">
</form>
<?php
if (isset($_POST['submit'])) {
  $n = $_POST['t1'];
  $a=0;
  $b=1;
  echo "the fibonacci series is:";
  echo $a;
  echo $b;
  for($i=2; $i <= $n; $i++){
  $c=$a+$b;
  echo $c;
  $a=$b;
  $b=$c;
  }
}
?>
</body>
</html>