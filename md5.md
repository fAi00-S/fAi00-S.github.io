# Hash PHP Function
## PHP MD5()
![](md5.jpg)

Message Digest Algorithm 5 หรือที่เรารู้จักกันดีในชื่อของ MD5 เป็นฟังก์ชันที่ใช้ในการเข้ารหัสชนิดหนึ่ง
โดยรูปแบบการเข้ารหัสเป็นแบบ Hashing Algorithm คือการเข้ารหัสข้อมูลที่มีความยาว 128 bits ให้ค่าเป็นตัวเลขฐาน 16
โดยที่ข้อมูลนั้นจะยาวหรือสั้น ก็จะถูกแปลงให้อยู่ในรูปแบบที่มีขนาดคงที่ คือขนาด 32 ตัวอักษร โดยมีการทำงานในลักษณะ 

## รูปแบบการใช้  MD5()
````PHP
md5(string, raw);
````
## พารามิเตอร์ 
|  Parameter  |                     Description                           |
|-------------|:---------------------------------------------------------:|
|string       |Required. The string to be calculated                      |
|raw          |Optional. Specify hex or binary output format:             |
|             |            TRUE - Raw 16 character binary format          |
|             |             FALSE - Default. 32 character hex number      |


## ตัวอย่างการใช้  MD5()
````PHP
<?php 
echo md5(Nantawan); 
?>
````
## ผลลัพธ์
````PHP
6b2ac01dcd137278d55abcd1ecb9417a
````

### ประโยชน์ของ md5()
ประโยชน์ของ Function md5() ที่สำคัญคือ สามารถใช้ในการตรวจสอบความถูกต้องของข้อมูลได้หรือในทาง Security เรียกว่า Integrity

## References:
- https://www.php.net/manual/en/function.md5.php

## Warning
`It is not recommended to use this function to secure passwords, due to the fast nature of this hashing algorithm. See the Password Hashing FAQ for details and best practices.`
