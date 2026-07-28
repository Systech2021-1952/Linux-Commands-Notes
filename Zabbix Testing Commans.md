# Install Zabbix Agent In Linux Agent Pc

Check the  Os version in zabbix server
> cat /etc/os-release

check the zabbix version in zabbix server
> zabbix_server --version


Check the Os version in linux  : 
> cat /etc/os-release

check linux os version
> hostnamectl


## Add Suse linux agent in zabbix server :

install zabix repo in linux agent :
> sudo rpm -Uvh https://repo.zabbix.com/zabbix/7.4/stable/sles/15/x86_64/zabbix-release-latest-7.4.sles15.noarch.rpm
> rpm -Uvh --nosignature https://repo.zabbix.com/zabbix/7.4/release/sles/15/noarch/zabbix-release-latest-7.4.sles15.noarch.rpm

Install Zabbix agent in linux :
> zypper install zabbix-agent


open zabbix file : 
> cd /etc/zabbix
> vi zabbix_agentd.conf

set zabbix server ip in linux 
> vi /etc/zabbix/zabbix_agentd.conf

## Add Zabbix Server IP & linux Agent hostname In Agent Pc :

> Server= YOUR_ZABBIX_SERVER_IP

> ServerActive= YOUR_ZABBIX_SERVER_IP

> Hostname= YOUR_LINUX_AGENT_HOSTNAME 

`````
ex:
#Server=192.168.1.9
#ServerActive=192.168.1.9
#Hostname=suse-prod-01

Save & Exit
Esc :wq 
`````

## Restart the Services : 

> systemctl enable zabbix-agent

> systemctl start zabbix-agent

> systemctl status zabbix-agent

----------

# Testing Commands 

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

## Completed


