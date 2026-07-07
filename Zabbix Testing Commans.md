```bash
cat /etc/os-release
cat -n /etc/zabbix/web/zabbix.conf.php
vi cat -n /etc/zabbix/web/zabbix.conf.php
vi /etc/zabbix/web/zabbix.conf.php
systemctl restart php-fpm nginx zabbix-server
systemctl status php-fpm nginx zabbix-server
systemctl status mysqld
df -h
dnf clean all
yum clean all
systemctl start mysqld
systemctl status mysqld
df -h
```


```
add linux agent in zabbix server

check Zabbix version in zabbix server
& 
check linux server agent

 cat /etc/os-release

 zypper install zabbix-agent

 vi /etc/zabbix/zabbix_agentd.conf
 	
 Server=YOUR_ZABBIX_SERVER_IP
ServerActive=YOUR_ZABBIX_SERVER_IP
Hostname=SUSE-SERVER


ex:
Server=192.168.1.10
ServerActive=192.168.1.10
Hostname=suse-prod-01

systemctl enable zabbix-agent
systemctl start zabbix-agent

systemctl status zabbix-agent



```
