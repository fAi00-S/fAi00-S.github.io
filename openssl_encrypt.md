# openssl_encrypt()
![](openssl.jpg)
ปกติเวลาเข้า website เราจะเรียกผ่าน URL ซึ่ง URL ที่ว่านี้ถ้าไม่มีการ design ด้าน security ซึ่งการรับส่งข้อมูลอาจไม่ไดเข้ารหัส session id
จึงเป็นช่องโหว่ให้ผู้ไม่ประสงค์ดี สุ่มเปลี่ยนแปลงเลข id เพื่อเข้าถึงข้อมูลในหน้าอื่นๆได้

และเพื่อแก้ไขช่องโหว่นี้ PHP มี Function openssl_encrypt เพื่อทำการเข้ารหัส session ไม่ให้สามารถอ่านหรือแก้ไข session ได้


`openssl_encrypt()` 

รูปแบบการใช้ function openssl_encrypt()
````PHP
$encrypted = openssl_encrypt($data, $method, $key);
````

ตัวอย่างการใช้ openssl_encrypt()
````PHP
$textToEncrypt = "My super secret information.";
$encryptionMethod = "AES-256-CBC";  // AES is used by the U.S. gov't to encrypt top secret documents.
$secretHash = "25c6c7ff35b9979b151f2136cd13b0ff";

//To encrypt
$encryptedMessage = openssl_encrypt($textToEncrypt, $encryptionMethod, $secretHash);

//To Decrypt
$decryptedMessage = openssl_decrypt($encryptedMessage, $encryptionMethod, $secretHash);

//Result
echo "Encrypted: $encryptedMessage <br>Decrypted: $decryptedMessage";
````

###References:
- https://www.php.net/manual/en/function.openssl-encrypt.php
- https://www.codegrepper.com/code-examples/php/php+openssl_encrypt
