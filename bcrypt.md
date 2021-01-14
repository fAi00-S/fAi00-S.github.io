# bcrypt() 
`Hash Algorithm` `bcrypt` `encryption` 
![](bcrypt.jpg)

เป็นการเข้าหัสแบบ `one-way hashing algorithm` คือไม่สามารถถอดให้เป็นแบบเดิมได้

เพราะใน algorithm มีการใช้ round เข้ามาด้วย ซึ่งต่างจาก `md5` หรือ `sha1` ที่จะได้ผลลัพธ์จากการเข้ารหัสเหมือนกันทุกๆ ครั้ง

## รูปแบบการใช้งาน
````PHP
$bcrypt = new Bcrypt(15);
$hash = $bcrypt->hash('password'); 
$check= $bcrypt->verify('password', $hash);
````
## ข้อดีของ bcrypt()
brute force ต้องใช้เวลานาน

