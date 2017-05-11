```
[root@ip-172-31-1-170 ec2-user]# beeline
Beeline version 1.1.0-cdh5.9.2 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-1-170.ap-southeast-1.compute.internal@SHAHUTSAV3988.COM
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-1-170.ap-southeast-1.compute.internal@SHAHUTSAV3988.COM
Connected to: Apache Hive (version 1.1.0-cdh5.9.2)
Driver: Hive JDBC (version 1.1.0-cdh5.9.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170510223636_a33bc124-ca63-440e-91d6-53f9aa1cca60): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170510223636_a33bc124-ca63-440e-91d6-53f9aa1cca60); Time taken: 0.736 seconds
INFO  : Executing command(queryId=hive_20170510223636_a33bc124-ca63-440e-91d6-53f9aa1cca60): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510223636_a33bc124-ca63-440e-91d6-53f9aa1cca60); Time taken: 0.302 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.409 seconds)
0: jdbc:hive2://localhost:10000/default> 
```
