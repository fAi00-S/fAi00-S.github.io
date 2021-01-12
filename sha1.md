<h1>Hash PHP Function</h1><br>
<h2>sha1() Function</h2><br>
<img src="sha1.jpg"  width="1069" height="300"><br>
Function Hash ใน PHP ไม่ได้มีแค่ md5() อย่างเดียวยังคงมี sha1() หรือชื่อเต็มของเค้าคือ Secure Hash Algorithm 1<br>
โดย sha1 จะมี Message Digest เท่ากับ 160 bits 

<h3>ตัวอย่าง</h3><br>
```php 
<?php 
$str = 'Hello';
echo sha1($str,FALSE);
?>
```

<h3>ผลลัพธ์</h3><br>
f7ff9e8b7bb2e09b70935a5d785e0cc5d9d0abf0<br>
ปัจจุบันการ hash ข้อมูลไม่แนะนำให้ใช้ทั้ง md5 และ sha1 แล้วเพราะ sha1 สามารถทำ Rainbow Table Crack<br>
และยังพบว่ามีการชนกันของ sha1 ซึ่งทำให้ Hash Function แบบ sha1 ไม่น่าเชื่อถือ<br>
