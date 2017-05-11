Test results of script 

```
[root@ip-172-31-1-170 ec2-user]# sh -x YARNTest.sh 
+ MR=/opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce
+ HADOOP=/opt/cloudera/parcels/CDH/bin
++ date
+ echo Testing loop started on Thu May 11 05:28:27 EDT 2017
Testing loop started on Thu May 11 05:28:27 EDT 2017
+ for i in 8
+ for j in 1
+ for k in 512 1024
++ echo '(512*0.8)/1'
++ bc
+ MAP_MB=409
++ echo '(512*0.8)/1'
++ bc
+ RED_MB=409
+ /opt/cloudera/parcels/CDH/bin/hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Dmapreduce.job.maps=8 -Dmapreduce.map.memory.mb=512 -Dmapreduce.map.java.opts.max.heap=409 51200000 /results/tg-10GB-8-1-512

real	1m13.765s
user	0m6.219s
sys	0m0.378s
+ /opt/cloudera/parcels/CDH/bin/hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort -Dmapreduce.job.maps=8 -Dmapreduce.job.reduces=1 -Dmapreduce.map.memory.mb=512 -Dmapreduce.map.java.opts.max.heap=409 -Dmapreduce.reduce.memory.mb=512 -Dmapreduce.reduce.java.opts.max.heap=409 /results/tg-10GB-8-1-512 /results/ts-10GB-8-1-512

real	2m32.880s
user	0m8.393s
sys	0m0.560s
+ /opt/cloudera/parcels/CDH/bin/hadoop fs -rm -r -skipTrash /results/tg-10GB-8-1-512
Deleted /results/tg-10GB-8-1-512
+ /opt/cloudera/parcels/CDH/bin/hadoop fs -rm -r -skipTrash /results/ts-10GB-8-1-512
Deleted /results/ts-10GB-8-1-512
+ for k in 512 1024
++ echo '(1024*0.8)/1'
++ bc
+ MAP_MB=819
++ echo '(1024*0.8)/1'
++ bc
+ RED_MB=819
+ /opt/cloudera/parcels/CDH/bin/hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen -Dmapreduce.job.maps=8 -Dmapreduce.map.memory.mb=1024 -Dmapreduce.map.java.opts.max.heap=819 51200000 /results/tg-10GB-8-1-1024

real	1m16.056s
user	0m6.218s
sys	0m0.379s
+ /opt/cloudera/parcels/CDH/bin/hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort -Dmapreduce.job.maps=8 -Dmapreduce.job.reduces=1 -Dmapreduce.map.memory.mb=1024 -Dmapreduce.map.java.opts.max.heap=819 -Dmapreduce.reduce.memory.mb=1024 -Dmapreduce.reduce.java.opts.max.heap=819 /results/tg-10GB-8-1-1024 /results/ts-10GB-8-1-1024

real	2m39.951s
user	0m8.596s
sys	0m0.506s
+ /opt/cloudera/parcels/CDH/bin/hadoop fs -rm -r -skipTrash /results/tg-10GB-8-1-1024
Deleted /results/tg-10GB-8-1-1024
+ /opt/cloudera/parcels/CDH/bin/hadoop fs -rm -r -skipTrash /results/ts-10GB-8-1-1024
Deleted /results/ts-10GB-8-1-1024
++ date
+ echo Testing loop ended on Thu May 11 05:36:23 EDT 2017
Testing loop ended on Thu May 11 05:36:23 EDT 2017

```

