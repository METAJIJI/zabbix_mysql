# Description
Extended monitoring mysql via zabbix agent.

# Dependencies
Required GNU awk, grep, mysqladmin.

Install packages if not installed.

For `deb` based e.g. ubuntu, debian:
```
apt-get install mysql-client-5.5
```

# Installation

```
mkdir /etc/zabbix/scripts
chown zabbix:zabbix /etc/zabbix/scripts
cp zabbix/scripts/mysql_status.sh /etc/zabbix/scripts
service zabbix-agent restart
```
Goto zabbix web gui and import template for you zabbix version from `template` directory.
