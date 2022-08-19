# How to convert ssl private-key.txt to private.key extension and PFX extension for ssl installation iis7 or iis10

## How to convert ssl private-key.txt to private.key extension

### Follow these steps below

1. Go to  https://www.openssl.org 

2. Download the openssl files

3. Extract the file under the folder C:\OpenSSL

4. Move C:\OpenSSL\bin\openssl.cnf to C:\OpenSSL\openssl.cnf

5. Now the Opensssl is installed

6. Now open the cmd and go to C:\OpenSSL\bin by using cd commands

7. then type openssl

8. Now type this command

9. openssl> rsa -in D:\sslfiles\private-key.txt -outform pem -out D:\sslfiles\private.key

10. Now Private Key is Generated fom the private-key.txt to pvt-key.key

## How to convert ssl CRT file PFX extension

11. Now create the PFX file by running following commands

12. pkcs12 -export -out D:\sslfiles\certi-ssl.pfx -inkey D:\sslfiles\private.key -in D:\sslfiles\cd0f163993d8bc38.crt

13. You can find the converted file in D:\sslfiles folder location.
