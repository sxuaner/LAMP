LAMP Server Setup
============
Installation and configuration of LAMP server. A security policy will be added later. Assuming we run all following commands as root.

Requirements:
------------
- RHEL 3.10.0-229.el7.x86_64
- MySql Ver 15.1 Distrib 5.5.42-MariaDB, for Linux (x86_64) using readline 5.1

HowTo
----------
###1. Repos needed. 
* Add MariaDB repo.
```ruby
   [mariadb]
   name = MariaDB
   baseurl = http://yum.mariadb.org/5.5/rhel6-amd64
   gpgkey=https://yum.mariadb.org/RPM-GPG-KEY-MariaDB
   gpgcheck=1
```
* [IUS Community Repo](http://wiki.centos.org/AdditionalResources/Repositories)
 provides the "latest upstream versions of PHP, Python, MySQL".

###2. Install MariaDB and Server
* On RHEL/CentOS 6/5 and Fedora 19,18,17:

        $ yum -y install MariaDB MariaDB-server

* On Fedora 20:

        $ yum -y install mariadb mariadb-server

###3. Start MariaDB:

        $ /etc/init.d/mysql start

###4. Install WordPress
         $ yum install wordpress

###5. Use phpMyAdmin to manage remote database

###6. Also, dont' forget to install php.

         CREATE USER 'jeffrey'@'localhost' IDENTIFIED BY 'mypass';
         
###7. phpMyAdmin config file :/etc/httpd/conf.d/phpMyAdmin.conf.
