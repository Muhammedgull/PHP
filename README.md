<html>
<head>
<meta charset="UTF-8">
<title>HTML - PHP</title>
</head>
<body>
<form action="" method="GET">
<input type="text" name="ad" placeholder="Adınızı Giriniz"><br>
<input type="text" name="soyad" placeholder="Soyadınızı Giriniz"><br>
ERKEK<input type="radio" name="cinsiyet" value="erkek"><br>
KADIN<input type="radio" name="cinsiyet" value="kadın"><br>
<input type="email" name="email" placeholder="example@email.com"><br>
<input type="submit" name="kaydet" value="kaydet">
<input type="submit" name="temizle" value="temizle">
</form>
<hr>

<?php
//eğer kaydet tıkandıysa
if(@$_GET["kaydet"]){
	echo "
	Ad: <b>$_GET[ad]</b><br>
	Soyad: <b>$_GET[soyad]</b><br>
	Cinsiyet: <b>$_GET[cinsiyet]</b><br>
	Email: <b>$_GET[email]</b><br>
	
	
	";

}else{
	echo "tiklanmadi.";
}

?>

</body>
</html>
