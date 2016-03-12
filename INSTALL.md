= Installation

== Debian and similar

As root

```bash
$ apt-get install mysql-server php5-adodb php5-mysql git # check or install dependencies
$ cd /var/www/html
$ git clone https://github.com/beastybeast/pcrypt.git # download pcrypt
$ chown -R www-data:www-data pcrypt
$ vim pcrypt/pcrypt.config.php # edit the file to match your settings
$ mysql -u root -p123456
mysql> create database pcrypt;
mysql> exit;
$ mysql -u root -ppassword pcrypt <passwordcrypt.sql
$ cd pcrypt
$ git clone https://github.com/acrylic/ADOdb_lite
$ mv ADOdb_lite adodb_lite
$ git clone https://github.com/PHPMailer/PHPMailer.git
$ mv PHPMailer phpmailer
```
