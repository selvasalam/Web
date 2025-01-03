<html>
<head>
</head>
<body>
<form method="post">
Enter a number:<input type="number" name="number" required><br>
<input type="submit" name="submit" value="Submit">
</form>
<?php
if(isset($_POST['submit'])){
$num=$_POST['number'];
$temp=$num;
$sum=0;

while($temp != 0){
$rem = $temp % 10;
$sum += $rem * $rem * $rem;
$temp = (int)($temp / 10);
}
if($num == $sum){
echo $num ."is an Amstrong number.";
}else{
echo $num."is not an Amstrong number.";
}
}
?>
<body>
</html