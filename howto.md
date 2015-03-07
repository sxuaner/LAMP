1. Add MariaDB repo

[mariadb]
name = MariaDB
baseurl = http://yum.mariadb.org/5.5/rhel6-amd64
gpgkey=https://yum.mariadb.org/RPM-GPG-KEY-MariaDB
gpgcheck=1

2. Install 
# On RHEL/CentOS 6/5 and Fedora 19,18,17 #
[root@tecmint]# yum -y install MariaDB MariaDB-server

# On Fedora 20 #
[root@tecmint]# yum -y install mariadb mariadb-server


3. /etc/init.d/mysql start


