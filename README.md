# XAMPP VHOST
---
## Download XAMPP
---
To download XAMPP [https://www.apachefriends.org/download.html]("https://www.apachefriends.org/download.html")

## Create VHOST
---
To create xampp vhost - go to xampp folder: C:\xampp\apache\conf\extra\httpd-vhosts.conf file, then add
```bash
<VirtualHost *:80>
    ServerAdmin webmaster@example.com
    DocumentRoot "C:/axmpp/htdoc/example.com"
    ServerName example.com
    ErrorLog "logs/example.com-error.log"
    CustomLog "logs/example.com-access.log" common

    <Directory "C:/axmpp/htdoc/example.com">
        Options Indexes
        AllowOverride All
        Require all granted
    </Directory>
</VirtualHost>
```