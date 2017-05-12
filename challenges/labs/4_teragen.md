```
[zhou@ip-172-31-10-8 ~]$ time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen  -D dfs.block.size=67108864 -Dmapreduce.job.maps=6 -Dmapreduce.map.memory.mb=1024 65536000 /user/zhou/tgen 1>tera_4_10.out 2>tera_4_10.err

```
```
real	1m12.849s
user	0m6.044s
sys	0m0.414s
[zhou@ip-172-31-10

```


```
[zhou@ip-172-31-10-8 ~]$ hdfs dfs -ls /user/zhou/tgen
Found 7 items
-rw-r--r--   3 zhou zhou          0 2017-05-11 23:47 /user/zhou/tgen/_SUCCESS
-rw-r--r--   3 zhou zhou 1092266700 2017-05-11 23:47 /user/zhou/tgen/part-m-00000
-rw-r--r--   3 zhou zhou 1092266700 2017-05-11 23:47 /user/zhou/tgen/part-m-00001
-rw-r--r--   3 zhou zhou 1092266600 2017-05-11 23:47 /user/zhou/tgen/part-m-00002
-rw-r--r--   3 zhou zhou 1092266700 2017-05-11 23:47 /user/zhou/tgen/part-m-00003
-rw-r--r--   3 zhou zhou 1092266700 2017-05-11 23:47 /user/zhou/tgen/part-m-00004
-rw-r--r--   3 zhou zhou 1092266600 2017-05-11 23:47 /user/zhou/tgen/part-m-00005
```
