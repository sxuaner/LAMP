LAMP Server Setup
============
Installation and configuration of LAMP server. A security policy will be added later.

Platforms
------------
- RHEL 3.10.0-229.el7.x86_64
- MySql Ver 15.1 Distrib 5.5.42-MariaDB, for Linux (x86_64) using readline 5.1

HowTo
----------

1. Add MariaDB repo.
   [mariadb]
   name = MariaDB
   baseurl = http://yum.mariadb.org/5.5/rhel6-amd64
   gpgkey=https://yum.mariadb.org/RPM-GPG-KEY-MariaDB
   gpgcheck=1

2. Install
- On RHEL/CentOS 6/5 and Fedora 19,18,17:

    $ yum -y install MariaDB MariaDB-server
- On Fedora 20:

        $ yum -y install mariadb mariadb-server

3. Start MariaDB:

        $ /etc/init.d/mysql start
