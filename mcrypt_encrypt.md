# PHP mcrypt_encrypt()
`encryption` 
![](mcrypt.jpg)


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
