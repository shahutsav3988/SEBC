

```
[root@ip-172-31-2-232 ec2-user]# ls /etc/yum.repos.d
redhat-rhui-client-config.repo  redhat.repo       rhui-load-balancers.conf
redhat-rhui.repo                rhel-source.repo

```


```
[root@ip-172-31-2-232 ec2-user]# /usr/share/cmf/schema/scm_prepare_database.sh mysql scm scm scm_password -h ip-172-31-10-8.ec2.internal -u root -p
Enter database password: 
JAVA_HOME=/usr/java/jdk1.7.0_67-cloudera
Verifying that we can write to /etc/cloudera-scm-server
[                          main] DbProvisioner                  ERROR Exception when creating/dropping database with user 'root' and jdbc url 'jdbc:mysql://ip-172-31-10-8.ec2.internal/?useUnicode=true&characterEncoding=UTF-8'
com.mysql.jdbc.exceptions.jdbc4.MySQLSyntaxErrorException: Access denied for user 'root'@'%' to database 'scm'
	at sun.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method)
	at sun.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:57)
	at sun.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45)
	at java.lang.reflect.Constructor.newInstance(Constructor.java:526)
	at com.mysql.jdbc.Util.handleNewInstance(Util.java:425)
	at com.mysql.jdbc.Util.getInstance(Util.java:408)
	at com.mysql.jdbc.SQLError.createSQLException(SQLError.java:943)
	at com.mysql.jdbc.MysqlIO.checkErrorPacket(MysqlIO.java:3973)
	at com.mysql.jdbc.MysqlIO.checkErrorPacket(MysqlIO.java:3909)
	at com.mysql.jdbc.MysqlIO.sendCommand(MysqlIO.java:2527)
	at com.mysql.jdbc.MysqlIO.sqlQueryDirect(MysqlIO.java:2680)
	at com.mysql.jdbc.ConnectionImpl.execSQL(ConnectionImpl.java:2486)
	at com.mysql.jdbc.ConnectionImpl.execSQL(ConnectionImpl.java:2444)
	at com.mysql.jdbc.StatementImpl.executeInternal(StatementImpl.java:845)
	at com.mysql.jdbc.StatementImpl.execute(StatementImpl.java:745)
	at com.cloudera.enterprise.dbutil.DbProvisioner.executeSql(DbProvisioner.java:286)
	at com.cloudera.enterprise.dbutil.DbProvisioner.doMain(DbProvisioner.java:95)
	at com.cloudera.enterprise.dbutil.DbProvisioner.main(DbProvisioner.java:110)
[                          main] DbProvisioner                  ERROR Stack Trace:
com.mysql.jdbc.exceptions.jdbc4.MySQLSyntaxErrorException: Access denied for user 'root'@'%' to database 'scm'
	at sun.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method)
	at sun.reflect.NativeConstructorAccessorImpl.newInstance(NativeConstructorAccessorImpl.java:57)
	at sun.reflect.DelegatingConstructorAccessorImpl.newInstance(DelegatingConstructorAccessorImpl.java:45)
	at java.lang.reflect.Constructor.newInstance(Constructor.java:526)
	at com.mysql.jdbc.Util.handleNewInstance(Util.java:425)
	at com.mysql.jdbc.Util.getInstance(Util.java:408)
	at com.mysql.jdbc.SQLError.createSQLException(SQLError.java:943)
	at com.mysql.jdbc.MysqlIO.checkErrorPacket(MysqlIO.java:3973)
	at com.mysql.jdbc.MysqlIO.checkErrorPacket(MysqlIO.java:3909)
	at com.mysql.jdbc.MysqlIO.sendCommand(MysqlIO.java:2527)
	at com.mysql.jdbc.MysqlIO.sqlQueryDirect(MysqlIO.java:2680)
	at com.mysql.jdbc.ConnectionImpl.execSQL(ConnectionImpl.java:2486)
	at com.mysql.jdbc.ConnectionImpl.execSQL(ConnectionImpl.java:2444)
	at com.mysql.jdbc.StatementImpl.executeInternal(StatementImpl.java:845)
	at com.mysql.jdbc.StatementImpl.execute(StatementImpl.java:745)
	at com.cloudera.enterprise.dbutil.DbProvisioner.executeSql(DbProvisioner.java:286)
	at com.cloudera.enterprise.dbutil.DbProvisioner.doMain(DbProvisioner.java:95)
	at com.cloudera.enterprise.dbutil.DbProvisioner.main(DbProvisioner.java:110)
--> Error 1, giving up (use --force if you wish to ignore the error)


```
