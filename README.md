<?php
$realname = $_POST["realname"];
$username = $_POST["username"];
$password = $_POST["password"];
$email = $_POST['email'];
 echo("$realname");


$link = mysqli_connect("localhost","root","","shop_db");
$query =" INSERT INTO `user_information` (realname,username, password, email, type) VALUES ('$realname', '$username', '$password', '$email', '0')"; 
mysqli_query($link,$query);



 mysqli_close($link);
?>
