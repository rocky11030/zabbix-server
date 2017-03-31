Table of Contents
=========

暂时只支持Centos7系统

数据库默认使用的是Mariadb

默认安装zabbix 3.0

```默认
---
- hosts: zabbix_server
  user: root
  roles:
    - role: ../../zabbix-server
      zabbix_apache_vhost_port: 80
      zabbix_url_aliases: []
      zabbix_version: 3.0
      zabbix_timezone: Asia/Shanghai
      zabbix_repo: zabbix
      zabbix_vhost: True
      zabbix_web: True
      zabbix_database_creation: True
      zabbix_database_sqlload: True
      database_type: mysql
      database_type_long: mysql
```
