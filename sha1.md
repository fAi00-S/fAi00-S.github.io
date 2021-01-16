# Hash PHP Function

## sha1() Function

![](sha1.jpg)
Function Hash ใน PHP ไม่ได้มีแค่ md5() อย่างเดียวยังคงมี sha1() หรือชื่อเต็มของเค้าคือ Secure Hash Algorithm 1
โดย sha1 จะมี Message Digest เท่ากับ 160 bits 

### ตัวอย่างการใช้ sha1()
 ````PHP
<?php<br>
$str = 'Hello';<br>
echo sha1($str,FALSE);<br>
?><br>
````

### ผลลัพธ์
 ````PHP
f7ff9e8b7bb2e09b70935a5d785e0cc5d9d0abf0
````

ปัจจุบันการ hash ข้อมูลไม่แนะนำให้ใช้ทั้ง md5 และ sha1 แล้วเพราะ sha1 สามารถทำ Rainbow Table Crack
และยังพบว่ามีการชนกันของ sha1 ซึ่งทำให้ Hash Function แบบ sha1 ไม่น่าเชื่อถือ

## References:
- https://www.php.net/manual/en/function.sha1.php
