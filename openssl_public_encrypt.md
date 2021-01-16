# openssl_public_encrypt()
`openssl` `openssl_public_encrypt` `encryption` 

![](opensslpublic.jpg)

รูปแบบการใช้ function openssl_public_encrypt()
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

### ตัวอย่างการใช้ openssl_public_encrypt()
````PHP
<?php
   // Save Private Key
   $privkey = openssl_pkey_new();
   openssl_pkey_export_to_file($privkey, 'C:/xampp/htdocs/modules/openssl/privatekey.pem');
	
   //Save Public Key
   $dn = array(
      "countryName" => "IN",
      "stateOrProvinceName" => "Karnataka",
      "localityName" => "test1",
      "organizationName" => "test2",
      "organizationalUnitName" => "test3",
      "commonName" => "www.test.com",
      "emailAddress" => "xyz@test.com"
   );
   $cert = openssl_csr_new($dn, $privkey);
   $cert = openssl_csr_sign($cert, null, $privkey, 365);
   openssl_x509_export_to_file($cert, 'C:/xampp/htdocs/modules/openssl/publickey.pem');
	
	
   // To encrpt data
   $data = 'Welcome To TuorialsPoint';
   $isvalid = openssl_public_encrypt ($data, $crypted , file_get_contents('C:/xampp/htdocs/modules/openssl/publickey.pem'),OPENSSL_PKCS1_PADDING);	
   echo "Data encryption : ".$crypted;
?>
````
### ผลลัพธ์
````PHP
Data encryption : ��E �wC�ݭ�+c��f*��o���W�7�EW��$�p�.rng�_N��A1��2Uݴ~s�ap۳)w��=� ��#��g;���u��_%�Z�bb�&��m��v&����q��k
````

### References:
- https://www.php.net/manual/en/function.openssl-public-encrypt.php
- https://www.tutorialspoint.com/php/php_function_openssl_public_encrypt.htm

