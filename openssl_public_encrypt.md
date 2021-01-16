# openssl_public_encrypt()
`openssl` `openssl_public_encrypt` `encryption` 

![](opensslpublic.jpg)

รูปแบบการใช้ function openssl_encrypt()
````PHP
openssl_public_encrypt ( string $data , string &$crypted , mixed $key , int $padding = OPENSSL_PKCS1_PADDING ) : bool
````
## พารามิเตอร์ 
|  Parameter  |                     Description                           |
|-------------|---------------------------------------------------------|
|data       |.                      |
|encrypted          |It will have the data that is encrypted.             |
|  key           |            The public key.         |
|     padding        |  The padding you can apply are : OPENSSL_PKCS1_PADDING, OPENSSL_SSLV23_PADDING, OPENSSL_PKCS1_OAEP_PADDING, OPENSSL_NO_PADDING.      |

ตัวอย่างการใช้ openssl_encrypt()
````PHP
openssl_public_encrypt ( string $data , string &$crypted , mixed $key , int $padding = OPENSSL_PKCS1_PADDING ) : bool
````

### References:
- https://www.php.net/manual/en/function.openssl-public-encrypt.php

