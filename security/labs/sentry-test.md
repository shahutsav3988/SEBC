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


George and Ferdinand


```
[root@ip-172-31-1-170 ec2-user]# beeline
Beeline version 1.1.0-cdh5.9.2 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-1-170.ap-southeast-1.compute.internal@SHAHUTSAV3988.COM
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-1-170.ap-southeast-1.compute.internal@SHAHUTSAV3988.COM
Connected to: Apache Hive (version 1.1.0-cdh5.9.2)
Driver: Hive JDBC (version 1.1.0-cdh5.9.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> CREATE ROLE reads;
INFO  : Compiling command(queryId=hive_20170510224545_3f5ffbd6-cda6-442d-a531-4c79c73e5af6): CREATE ROLE reads
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224545_3f5ffbd6-cda6-442d-a531-4c79c73e5af6); Time taken: 0.08 seconds
INFO  : Executing command(queryId=hive_20170510224545_3f5ffbd6-cda6-442d-a531-4c79c73e5af6): CREATE ROLE reads
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224545_3f5ffbd6-cda6-442d-a531-4c79c73e5af6); Time taken: 0.046 seconds
INFO  : OK
No rows affected (0.191 seconds)
0: jdbc:hive2://localhost:10000/default> CREATE ROLE writes;
INFO  : Compiling command(queryId=hive_20170510224545_57eefe5f-ad61-4902-862c-84535806f480): CREATE ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224545_57eefe5f-ad61-4902-862c-84535806f480); Time taken: 0.057 seconds
INFO  : Executing command(queryId=hive_20170510224545_57eefe5f-ad61-4902-862c-84535806f480): CREATE ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224545_57eefe5f-ad61-4902-862c-84535806f480); Time taken: 0.027 seconds
INFO  : OK
No rows affected (0.098 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT SELECT ON DATABASE default TO ROLE reads;
INFO  : Compiling command(queryId=hive_20170510224545_1c54289c-824e-4618-9095-8a25c07e92a3): GRANT SELECT ON DATABASE default TO ROLE reads
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224545_1c54289c-824e-4618-9095-8a25c07e92a3); Time taken: 0.067 seconds
INFO  : Executing command(queryId=hive_20170510224545_1c54289c-824e-4618-9095-8a25c07e92a3): GRANT SELECT ON DATABASE default TO ROLE reads
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224545_1c54289c-824e-4618-9095-8a25c07e92a3); Time taken: 0.046 seconds
INFO  : OK
No rows affected (0.127 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT ROLE reads TO GROUP selector;
INFO  : Compiling command(queryId=hive_20170510224545_8ef541b0-ffce-42b1-972c-f20ed3b350f6): GRANT ROLE reads TO GROUP selector
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224545_8ef541b0-ffce-42b1-972c-f20ed3b350f6); Time taken: 0.058 seconds
INFO  : Executing command(queryId=hive_20170510224545_8ef541b0-ffce-42b1-972c-f20ed3b350f6): GRANT ROLE reads TO GROUP selector
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224545_8ef541b0-ffce-42b1-972c-f20ed3b350f6); Time taken: 0.03 seconds
INFO  : OK
No rows affected (0.104 seconds)
0: jdbc:hive2://localhost:10000/default> REVOKE ALL ON DATABASE default FROM ROLE writes;
INFO  : Compiling command(queryId=hive_20170510224545_fa36f391-fb6e-4d1e-ba9a-02ab07a60edd): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224545_fa36f391-fb6e-4d1e-ba9a-02ab07a60edd); Time taken: 0.057 seconds
INFO  : Executing command(queryId=hive_20170510224545_fa36f391-fb6e-4d1e-ba9a-02ab07a60edd): REVOKE ALL ON DATABASE default FROM ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224545_fa36f391-fb6e-4d1e-ba9a-02ab07a60edd); Time taken: 0.098 seconds
INFO  : OK
No rows affected (0.169 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT SELECT ON default.sample_07 TO ROLE writes;
INFO  : Compiling command(queryId=hive_20170510224545_e367c519-793f-4b82-9add-9484ad7841f2): GRANT SELECT ON default.sample_07 TO ROLE writes
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224545_e367c519-793f-4b82-9add-9484ad7841f2); Time taken: 0.076 seconds
INFO  : Executing command(queryId=hive_20170510224545_e367c519-793f-4b82-9add-9484ad7841f2): GRANT SELECT ON default.sample_07 TO ROLE writes
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224545_e367c519-793f-4b82-9add-9484ad7841f2); Time taken: 0.044 seconds
INFO  : OK
No rows affected (0.136 seconds)
0: jdbc:hive2://localhost:10000/default> GRANT ROLE writes TO GROUP inserters;
INFO  : Compiling command(queryId=hive_20170510224646_c6f8c20d-0b7b-41e2-8bfa-97df736dae07): GRANT ROLE writes TO GROUP inserters
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:null, properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224646_c6f8c20d-0b7b-41e2-8bfa-97df736dae07); Time taken: 0.056 seconds
INFO  : Executing command(queryId=hive_20170510224646_c6f8c20d-0b7b-41e2-8bfa-97df736dae07): GRANT ROLE writes TO GROUP inserters
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224646_c6f8c20d-0b7b-41e2-8bfa-97df736dae07); Time taken: 0.028 seconds
INFO  : OK
No rows affected (0.099 seconds)
0: jdbc:hive2://localhost:10000/default> quit;
Error: Error while compiling statement: FAILED: ParseException line 1:0 cannot recognize input near 'quit' '<EOF>' '<EOF>' (state=42000,code=40000)
0: jdbc:hive2://localhost:10000/default> quit
. . . . . . . . . . . . . . . . . . . .> exit
. . . . . . . . . . . . . . . . . . . .> 
. . . . . . . . . . . . . . . . . . . .> 
. . . . . . . . . . . . . . . . . . . .> bye
. . . . . . . . . . . . . . . . . . . .> [root@ip-172-31-1-170 ec2-user]# 
[root@ip-172-31-1-170 ec2-user]# 
[root@ip-172-31-1-170 ec2-user]# 
[root@ip-172-31-1-170 ec2-user]# 
[root@ip-172-31-1-170 ec2-user]# kinit george
Password for george@SHAHUTSAV3988.COM: 
[root@ip-172-31-1-170 ec2-user]# beeline
Beeline version 1.1.0-cdh5.9.2 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-1-170.ap-southeast-1.compute.internal@SHAHUTSAV3988.COM
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-1-170.ap-southeast-1.compute.internal@SHAHUTSAV3988.COM
Connected to: Apache Hive (version 1.1.0-cdh5.9.2)
Driver: Hive JDBC (version 1.1.0-cdh5.9.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170510224747_dcbfbd6e-01e0-4986-a3ae-f613302cef17): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224747_dcbfbd6e-01e0-4986-a3ae-f613302cef17); Time taken: 0.075 seconds
INFO  : Executing command(queryId=hive_20170510224747_dcbfbd6e-01e0-4986-a3ae-f613302cef17): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224747_dcbfbd6e-01e0-4986-a3ae-f613302cef17); Time taken: 0.14 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| customers  |
| emp        |
| sample_07  |
| sample_08  |
| web_logs   |
+------------+--+
5 rows selected (0.374 seconds)
0: jdbc:hive2://localhost:10000/default> 


[root@ip-172-31-1-170 ec2-user]# kinit ferdinand
Password for ferdinand@SHAHUTSAV3988.COM: 
kinit: Password incorrect while getting initial credentials
[root@ip-172-31-1-170 ec2-user]# kinit ferdinand
Password for ferdinand@SHAHUTSAV3988.COM: 
[root@ip-172-31-1-170 ec2-user]# beeline
Beeline version 1.1.0-cdh5.9.2 by Apache Hive
beeline> !connect jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-1-170.ap-southeast-1.compute.internal@SHAHUTSAV3988.COM
scan complete in 2ms
Connecting to jdbc:hive2://localhost:10000/default;principal=hive/ip-172-31-1-170.ap-southeast-1.compute.internal@SHAHUTSAV3988.COM
Connected to: Apache Hive (version 1.1.0-cdh5.9.2)
Driver: Hive JDBC (version 1.1.0-cdh5.9.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://localhost:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170510224949_e191c7ba-e32c-4226-9d86-11f53f49f3e6): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170510224949_e191c7ba-e32c-4226-9d86-11f53f49f3e6); Time taken: 0.074 seconds
INFO  : Executing command(queryId=hive_20170510224949_e191c7ba-e32c-4226-9d86-11f53f49f3e6): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510224949_e191c7ba-e32c-4226-9d86-11f53f49f3e6); Time taken: 0.146 seconds
INFO  : OK
+------------+--+
|  tab_name  |
+------------+--+
| sample_07  |
+------------+--+
1 row selected (0.318 seconds)
0: jdbc:hive2://localhost:10000/default>
```
