

```
wget http://repo.mysql.com/mysql-community-release-el6-7.noarch.rpm
```

```
[root@ip-172-31-10-8 ec2-user]# yum repolist all | grep mysql
Failed to set locale, defaulting to C
mysql-connectors-community                       MySQL Connectors enabled:    36
mysql-connectors-community-source                MySQL Connectors disabled
mysql-tools-community                            MySQL Tools Comm enabled:    47
mysql-tools-community-source                     MySQL Tools Comm disabled
mysql55-community                                MySQL 5.5 Commun disabled
mysql55-community-source                         MySQL 5.5 Commun disabled
mysql56-community                                MySQL 5.6 Commun enabled:   358
mysql56-community-source                         MySQL 5.6 Commun disabled
mysql57-community                                MySQL 5.7 Commun disabled
mysql57-community-source                         MySQL 5.7 Commun disabled
```

```
hostname -f
ip-172-31-10-8.ec2.internal

```

```
mysql --version
mysql  Ver 14.14 Distrib 5.6.36, for Linux (x86_64) using  EditLine wrapper

```


```
mysql> show databases;
+--------------------+
| Database           |
+--------------------+
| information_schema |
| amon               |
| hue                |
| metastore          |
| mysql              |
| oozie              |
| performance_schema |
| rman               |
| sentry             |
+--------------------+
9 rows in set (0.00 sec)

mysql> 

```
