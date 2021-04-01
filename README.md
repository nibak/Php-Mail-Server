# Php-Mail-Server
This project contains the configuration file for setting up your php mail server. This procedure is without using the Mercury from the XAMPP. It is very simple and easy to set up.
# Requirement
•	XAMPP 
•	G-mail enabled with “Less Secured Apps”.

# File changes
There are certain commands that needs to be updated in few files. Or you can download the files I have uploaded and apply the main changes
## php.ini
File Location= C:\xampp\php
Changes:
[mail function]
; For Win32 only.
; http://php.net/smtp
SMTP=smtp.gmail.com
; http://php.net/smtp-port
smtp_port=587

[OpenSSL]
ini_set("SMTP","ssl://smtp.gmail.com");
ini_set("smtp_port","587");
openssl.cafile="C:\xampp\apache\bin\curl-ca-bundle.crt"


## sendmail
