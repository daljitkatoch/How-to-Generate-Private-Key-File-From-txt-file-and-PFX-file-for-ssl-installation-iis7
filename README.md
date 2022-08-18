# How to Generate Private Key File From txt file and PFX file for ssl installation iis7
## How to Convert private-key.txt file to private-key.key

Go to  https://www.openssl.org 

Download the openssl files

Extract the file under the folder C:\OpenSSL

Move C:\OpenSSL\bin\openssl.cnf to C:\OpenSSL\openssl.cnf

Now the Opensssl is installed

Now open the cmd and go to C:\OpenSSL\bin by using cd commands

then type openssl

Now type this command

openssl> rsa -in D:\sslfiles\private-key.txt -outform pem -out D:\sslfiles\pvt-key.key

Now Private Key is Generated fom the private-key.txt to pvt-key.key

Now create the PFX file by running following commands

pkcs12 -export -out F:\sslfiles\certi-ssl.pfx -inkey F:\sslfiles\pvt-key.key -in F:\sslfiles\cd0f163993d8bc38.crt
