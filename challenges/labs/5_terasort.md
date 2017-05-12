
```

time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort /user/zhou/tgen/ /user/zhou/tsot 1>ts_10.out 2>ts_10.err

```

```
[root@ip-172-31-2-232 zhou]# time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort /user/zhou/tgen/ /user/zhou/tsot 1>ts_10.out 2>ts_10.err

real	2m46.919s
user	0m8.311s
sys	0m0.447s

```

```

[root@ip-172-31-2-232 zhou]# cat ts_10.err 
17/05/12 00:28:29 INFO terasort.TeraSort: starting
17/05/12 00:28:30 INFO hdfs.DFSClient: Created token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@SHAHUTSAV3988.CN, renewer=yarn, realUser=, issueDate=1494563310728, maxDate=1495168110728, sequenceNumber=1, masterKeyId=2 on 172.31.10.8:8020
17/05/12 00:28:30 INFO security.TokenCache: Got dt for hdfs://ip-172-31-10-8.ec2.internal:8020; Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.10.8:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@SHAHUTSAV3988.CN, renewer=yarn, realUser=, issueDate=1494563310728, maxDate=1495168110728, sequenceNumber=1, masterKeyId=2)
17/05/12 00:28:30 INFO input.FileInputFormat: Total input paths to process : 6
17/05/12 00:28:31 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-10-8.ec2.internal/172.31.10.8:8032
17/05/12 00:28:32 INFO mapreduce.JobSubmitter: number of splits:102
17/05/12 00:28:32 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494563203488_0001
17/05/12 00:28:32 INFO mapreduce.JobSubmitter: Kind: HDFS_DELEGATION_TOKEN, Service: 172.31.10.8:8020, Ident: (token for zhou: HDFS_DELEGATION_TOKEN owner=zhou@SHAHUTSAV3988.CN, renewer=yarn, realUser=, issueDate=1494563310728, maxDate=1495168110728, sequenceNumber=1, masterKeyId=2)
17/05/12 00:28:33 INFO impl.YarnClientImpl: Submitted application application_1494563203488_0001
17/05/12 00:28:33 INFO mapreduce.Job: The url to track the job: http://ip-172-31-10-8.ec2.internal:8088/proxy/application_1494563203488_0001/
17/05/12 00:28:33 INFO mapreduce.Job: Running job: job_1494563203488_0001
17/05/12 00:28:42 INFO mapreduce.Job: Job job_1494563203488_0001 running in uber mode : false
17/05/12 00:28:42 INFO mapreduce.Job:  map 0% reduce 0%
17/05/12 00:28:50 INFO mapreduce.Job:  map 1% reduce 0%
17/05/12 00:28:55 INFO mapreduce.Job:  map 3% reduce 0%
17/05/12 00:28:58 INFO mapreduce.Job:  map 4% reduce 0%
17/05/12 00:29:00 INFO mapreduce.Job:  map 5% reduce 0%
17/05/12 00:29:01 INFO mapreduce.Job:  map 6% reduce 0%
17/05/12 00:29:02 INFO mapreduce.Job:  map 11% reduce 0%
17/05/12 00:29:03 INFO mapreduce.Job:  map 12% reduce 0%
17/05/12 00:29:05 INFO mapreduce.Job:  map 13% reduce 0%
17/05/12 00:29:09 INFO mapreduce.Job:  map 15% reduce 0%
17/05/12 00:29:11 INFO mapreduce.Job:  map 16% reduce 0%
17/05/12 00:29:12 INFO mapreduce.Job:  map 19% reduce 0%
17/05/12 00:29:13 INFO mapreduce.Job:  map 22% reduce 0%
17/05/12 00:29:16 INFO mapreduce.Job:  map 23% reduce 0%
17/05/12 00:29:17 INFO mapreduce.Job:  map 24% reduce 0%
17/05/12 00:29:19 INFO mapreduce.Job:  map 25% reduce 0%
17/05/12 00:29:23 INFO mapreduce.Job:  map 28% reduce 0%
17/05/12 00:29:24 INFO mapreduce.Job:  map 31% reduce 0%
17/05/12 00:29:25 INFO mapreduce.Job:  map 32% reduce 0%
17/05/12 00:29:26 INFO mapreduce.Job:  map 33% reduce 0%
17/05/12 00:29:30 INFO mapreduce.Job:  map 34% reduce 0%
17/05/12 00:29:32 INFO mapreduce.Job:  map 36% reduce 0%
17/05/12 00:29:33 INFO mapreduce.Job:  map 38% reduce 0%
17/05/12 00:29:34 INFO mapreduce.Job:  map 39% reduce 0%
17/05/12 00:29:35 INFO mapreduce.Job:  map 41% reduce 0%
17/05/12 00:29:36 INFO mapreduce.Job:  map 42% reduce 0%
17/05/12 00:29:37 INFO mapreduce.Job:  map 43% reduce 0%
17/05/12 00:29:39 INFO mapreduce.Job:  map 44% reduce 0%
17/05/12 00:29:40 INFO mapreduce.Job:  map 45% reduce 0%
17/05/12 00:29:43 INFO mapreduce.Job:  map 46% reduce 0%
17/05/12 00:29:44 INFO mapreduce.Job:  map 48% reduce 0%
17/05/12 00:29:45 INFO mapreduce.Job:  map 50% reduce 0%
17/05/12 00:29:46 INFO mapreduce.Job:  map 51% reduce 0%
17/05/12 00:29:47 INFO mapreduce.Job:  map 54% reduce 0%
17/05/12 00:29:51 INFO mapreduce.Job:  map 55% reduce 0%
17/05/12 00:29:53 INFO mapreduce.Job:  map 56% reduce 0%
17/05/12 00:29:54 INFO mapreduce.Job:  map 58% reduce 0%
17/05/12 00:29:55 INFO mapreduce.Job:  map 59% reduce 0%
17/05/12 00:29:56 INFO mapreduce.Job:  map 60% reduce 0%
17/05/12 00:29:57 INFO mapreduce.Job:  map 63% reduce 0%
17/05/12 00:29:58 INFO mapreduce.Job:  map 64% reduce 0%
17/05/12 00:30:01 INFO mapreduce.Job:  map 66% reduce 0%
17/05/12 00:30:04 INFO mapreduce.Job:  map 67% reduce 0%
17/05/12 00:30:05 INFO mapreduce.Job:  map 68% reduce 0%
17/05/12 00:30:06 INFO mapreduce.Job:  map 69% reduce 0%
17/05/12 00:30:07 INFO mapreduce.Job:  map 71% reduce 0%
17/05/12 00:30:08 INFO mapreduce.Job:  map 75% reduce 0%
17/05/12 00:30:14 INFO mapreduce.Job:  map 76% reduce 0%
17/05/12 00:30:15 INFO mapreduce.Job:  map 78% reduce 0%
17/05/12 00:30:17 INFO mapreduce.Job:  map 79% reduce 0%
17/05/12 00:30:18 INFO mapreduce.Job:  map 81% reduce 0%
17/05/12 00:30:19 INFO mapreduce.Job:  map 84% reduce 0%
17/05/12 00:30:22 INFO mapreduce.Job:  map 86% reduce 0%
17/05/12 00:30:24 INFO mapreduce.Job:  map 87% reduce 0%
17/05/12 00:30:26 INFO mapreduce.Job:  map 89% reduce 0%
17/05/12 00:30:28 INFO mapreduce.Job:  map 90% reduce 0%
17/05/12 00:30:29 INFO mapreduce.Job:  map 93% reduce 0%
17/05/12 00:30:31 INFO mapreduce.Job:  map 93% reduce 3%
17/05/12 00:30:32 INFO mapreduce.Job:  map 93% reduce 6%
17/05/12 00:30:35 INFO mapreduce.Job:  map 94% reduce 6%
17/05/12 00:30:36 INFO mapreduce.Job:  map 95% reduce 12%
17/05/12 00:30:37 INFO mapreduce.Job:  map 96% reduce 13%
17/05/12 00:30:38 INFO mapreduce.Job:  map 97% reduce 16%
17/05/12 00:30:40 INFO mapreduce.Job:  map 98% reduce 16%
17/05/12 00:30:43 INFO mapreduce.Job:  map 100% reduce 16%
17/05/12 00:30:45 INFO mapreduce.Job:  map 100% reduce 18%
17/05/12 00:30:46 INFO mapreduce.Job:  map 100% reduce 20%
17/05/12 00:30:47 INFO mapreduce.Job:  map 100% reduce 26%
17/05/12 00:30:48 INFO mapreduce.Job:  map 100% reduce 31%
17/05/12 00:30:49 INFO mapreduce.Job:  map 100% reduce 32%
17/05/12 00:30:50 INFO mapreduce.Job:  map 100% reduce 33%
17/05/12 00:30:51 INFO mapreduce.Job:  map 100% reduce 41%
17/05/12 00:30:52 INFO mapreduce.Job:  map 100% reduce 44%
17/05/12 00:30:53 INFO mapreduce.Job:  map 100% reduce 49%
17/05/12 00:30:54 INFO mapreduce.Job:  map 100% reduce 53%
17/05/12 00:30:55 INFO mapreduce.Job:  map 100% reduce 56%
17/05/12 00:30:56 INFO mapreduce.Job:  map 100% reduce 60%
17/05/12 00:30:57 INFO mapreduce.Job:  map 100% reduce 63%
17/05/12 00:30:58 INFO mapreduce.Job:  map 100% reduce 67%
17/05/12 00:30:59 INFO mapreduce.Job:  map 100% reduce 71%
17/05/12 00:31:00 INFO mapreduce.Job:  map 100% reduce 73%
17/05/12 00:31:01 INFO mapreduce.Job:  map 100% reduce 74%
17/05/12 00:31:02 INFO mapreduce.Job:  map 100% reduce 78%
17/05/12 00:31:03 INFO mapreduce.Job:  map 100% reduce 79%
17/05/12 00:31:04 INFO mapreduce.Job:  map 100% reduce 87%
17/05/12 00:31:05 INFO mapreduce.Job:  map 100% reduce 88%
17/05/12 00:31:07 INFO mapreduce.Job:  map 100% reduce 94%
17/05/12 00:31:09 INFO mapreduce.Job:  map 100% reduce 95%
17/05/12 00:31:10 INFO mapreduce.Job:  map 100% reduce 98%
17/05/12 00:31:11 INFO mapreduce.Job:  map 100% reduce 99%
17/05/12 00:31:13 INFO mapreduce.Job:  map 100% reduce 100%
17/05/12 00:31:14 INFO mapreduce.Job: Job job_1494563203488_0001 completed successfully
17/05/12 00:31:14 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=2931170167
		FILE: Number of bytes written=5818254603
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=6553613464
		HDFS: Number of bytes written=6553600000
		HDFS: Number of read operations=336
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=20
	Job Counters 
		Launched map tasks=102
		Launched reduce tasks=10
		Data-local map tasks=100
		Rack-local map tasks=2
		Total time spent by all maps in occupied slots (ms)=851689
		Total time spent by all reduces in occupied slots (ms)=298480
		Total time spent by all map tasks (ms)=851689
		Total time spent by all reduce tasks (ms)=298480
		Total vcore-seconds taken by all map tasks=851689
		Total vcore-seconds taken by all reduce tasks=298480
		Total megabyte-seconds taken by all map tasks=872129536
		Total megabyte-seconds taken by all reduce tasks=305643520
	Map-Reduce Framework
		Map input records=65536000
		Map output records=65536000
		Map output bytes=6684672000
		Map output materialized bytes=2873077438
		Input split bytes=13464
		Combine input records=0
		Combine output records=0
		Reduce input groups=65536000
		Reduce shuffle bytes=2873077438
		Reduce input records=65536000
		Reduce output records=65536000
		Spilled Records=131072000
		Shuffled Maps =1020
		Failed Shuffles=0
		Merged Map outputs=1020
		GC time elapsed (ms)=16561
		CPU time spent (ms)=699980
		Physical memory (bytes) snapshot=59864297472
		Virtual memory (bytes) snapshot=175603478528
		Total committed heap usage (bytes)=66332917760
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=6553600000
	File Output Format Counters 
		Bytes Written=6553600000

```

