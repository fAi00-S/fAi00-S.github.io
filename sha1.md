<h1>Hash PHP Function</h1><br>
<h3>sha1()</h3><br>
<img src="sha1.jpg"  width="1069" height="300"><br>
Function Hash ใน PHP ไม่ได้มีแค่ md5() อย่างเดียวยังคงมี sha1() หรือชื่อเต็มของเค้าคือ Secure Hash Algorithm 1<br>
โดย sha1()

  <h3>ตัวอย่าง</h3><br>
<?php
$str = 'Hello';
echo sha1($str,FALSE);
?>

<h3>ผลลัพธ์</h3><br>
f7ff9e8b7bb2e09b70935a5d785e0cc5d9d0abf0
