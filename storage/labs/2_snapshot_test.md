
Create a precious directory in HDFS; copy the ZIP course file into it.
```
[shahutsav3988@ip-172-31-1-170 ~]$ wget https://github.com/shahutsav3988/SEBC/archive/master.zip
--2017-05-10 04:39:47--  https://github.com/shahutsav3988/SEBC/archive/master.zip
Resolving github.com... 192.30.255.112, 192.30.255.113
Connecting to github.com|192.30.255.112|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://codeload.github.com/shahutsav3988/SEBC/zip/master [following]
--2017-05-10 04:39:48--  https://codeload.github.com/shahutsav3988/SEBC/zip/master
Resolving codeload.github.com... 192.30.253.120, 192.30.253.121
Connecting to codeload.github.com|192.30.253.120|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1410278 (1.3M) [application/zip]
Saving to: `master.zip'

100%[====================================================================================================================================================================================================>] 1,410,278    433K/s   in 3.2s    

2017-05-10 04:39:52 (433 KB/s) - `master.zip' saved [1410278/1410278]

[shahutsav3988@ip-172-31-1-170 ~]$ hdfs dfs -mkdir /user/shahutsav3988/precious
[shahutsav3988@ip-172-31-1-170 ~]$ hdfs dfs -put master.zip /user/shahutsav3988/precious/

```

Enable snapshots for precious

```
hdfs dfsadmin -allowSnapshot /user/shahutsav3988/precious
Allowing snaphot on /user/shahutsav3988/precious succeeded
```
Create a snapshot called sebc-hdfs-test

```
[hdfs@ip-172-31-1-170 yum.repos.d]$ hdfs dfs -createSnapshot /user/shahutsav3988/precious sebc-hdfs-test
Created snapshot /user/shahutsav3988/precious/.snapshot/sebc-hdfs-test
```
