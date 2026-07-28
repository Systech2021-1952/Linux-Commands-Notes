# Install Zabbix Agent In Linux Agent Pc

check the zabbix version in zabbix server
> #zabbix_server --version

Check the  Os version in linux agent : 
> #cat /etc/os-release

check linux agent os version
> #hostnamectl


## Add Suse linux agent in zabbix server :
install zabix repo in linux agent :
> sudo rpm -Uvh https://repo.zabbix.com/zabbix/7.4/stable/sles/15/x86_64/zabbix-release-latest-7.4.sles15.noarch.rpm
> rpm -Uvh --nosignature https://repo.zabbix.com/zabbix/7.4/release/sles/15/noarch/zabbix-release-latest-7.4.sles15.noarch.rpm


> cat -n /etc/zabbix/web/zabbix.conf.php
>
> vi cat -n /etc/zabbix/web/zabbix.conf.php
>
> vi /etc/zabbix/web/zabbix.conf.php
>
> systemctl restart php-fpm nginx zabbix-server
>
> systemctl status php-fpm nginx zabbix-server
>
> systemctl status mysqld
>
> df -h
>
> dnf clean all
>
> yum clean all
>
> systemctl start mysqld
>
> systemctl status mysqld
>
> df -h
----------

## Add Suse linux agent in zabbix server :

check Zabbix version in zabbix server : 
& 
check linux server agent :

 cat /etc/os-release


Install Zabbix agent in linux :
 zypper install zabbix-agent

set zabbix server ip in linux 
 vi /etc/zabbix/zabbix_agentd.conf

> Server=YOUR_ZABBIX_SERVER_IP
> ServerActive=YOUR_ZABBIX_SERVER_IP
> Hostname=SUSE-SERVER (linux agent hostname)
````
----------
> ex:
> 
> Server=192.168.1.10
>
> ServerActive=192.168.1.10
>
> Hostname=suse-prod-01
>
> systemctl enable zabbix-agent
>
> systemctl start zabbix-agent
>
> systemctl status zabbix-agent

----------
## Completed


