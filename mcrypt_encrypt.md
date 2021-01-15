# PHP mcrypt_encrypt()
`encryption` `Symmetric Encryption` `Secret  Key` `Cipher Text`
![](mcrypt.jpg)

ด้วยยุค Digital ณ ปัจจุบัน อะไรๆ ก็ online กันทั้งนั้น ซึ่งนั้นทำให้ทุกอย่างทำผ่าน website หรือ Application
โดยที่ต้องมีการกรอกข้อมูลมากมายลงไป แล้วเราจะมั่นใจได้อย่างไรว่า ข้อมูลที่กรอกไปนั้นปลอดภัย
ดังนั้นนักพัฒนาต้องทำการ Encryption ข้อมูลเพื่อไม่ให้ผู้ไม่ประสงค์ดีสามารถอ่านข้อมูลที่เป็นได้
โดยการนำข้อความ `Plain text`  ที่จะต้องการส่ง มา `Encryption` ซึ่งจะได้มีข้อความที่จะต้องถูกเข้ารหัส หรือ `Cipher Text` 
ด้วยการเข้ารหัสในแบบสมมาตร ที่เรียกกันว่า Symmetric Encryption หรือ  Secret  Key เป็นการใช้ Key ลับของผู้เข้ารหัส ซึ่งคนที่จะถอดรหัสได้ ก็ต้องใช้ Key เดียวกัน

## รูปแบบการใช้ mcrypt_encrypt()
````PHP
mcrypt_encrypt ( string $cipher , string $key , string $data , string $mode , string $iv = ? ) : string|false
````
## ตัวอย่าง
````PHP
<?php

  $data = Nantawan Sanpukdee';

  $key = 'utrdn6kcxkfgs6keo23345kfniomgf4s';
  $suffix = '4678965001980654';

  $code = mcrypt_encrypt(MCRYPT_RIJNDAEL_128, $key, $data, MCRYPT_MODE_CFB, $suffix); 
  echo $code; 
  exit;

?>
````

## References:
- https://www.php.net/manual/en/function.openssl-encrypt.php

## Warning
`This function has been DEPRECATED as of PHP 7.1.0 and REMOVED as of PHP 7.2.0. Relying on this function is highly discouraged.`
