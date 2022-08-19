# How to convert ssl private-key.txt to private.key extension and PFX extension for ssl installation iis7 or iis10

## How to convert ssl private-key.txt to private.key extension

Go to  https://www.openssl.org 

Download the openssl files

Extract the file under the folder C:\OpenSSL

Move C:\OpenSSL\bin\openssl.cnf to C:\OpenSSL\openssl.cnf

Now the Opensssl is installed

Now open the cmd and go to C:\OpenSSL\bin by using cd commands

then type openssl

Now type this command

openssl> rsa -in D:\sslfiles\private-key.txt -outform pem -out D:\sslfiles\private.key

Now Private Key is Generated fom the private-key.txt to pvt-key.key

## How to convert ssl CRT file PFX extension

Now create the PFX file by running following commands

pkcs12 -export -out F:\sslfiles\certi-ssl.pfx -inkey F:\sslfiles\private.key -in F:\sslfiles\cd0f163993d8bc38.crt
