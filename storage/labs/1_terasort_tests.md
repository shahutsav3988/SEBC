The full teragen and command you used and the job output

```
time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar teragen  -D dfs.block.size=33554432 -Dmapreduce.job.maps=4 100000000 /user/shahutsav3988/tg-10GB-4 1>tera_4_10.out 2>tera_4_10.err

real	2m13.556s
user	0m6.646s
sys	0m0.447s


17/05/10 04:15:48 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-1-170.ap-southeast-1.compute.internal/172.31.1.170:8032
17/05/10 04:15:49 INFO terasort.TeraSort: Generating 100000000 using 4
17/05/10 04:15:49 INFO mapreduce.JobSubmitter: number of splits:4
17/05/10 04:15:49 INFO Configuration.deprecation: dfs.block.size is deprecated. Instead, use dfs.blocksize
17/05/10 04:15:49 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494400291896_0002
17/05/10 04:15:49 INFO impl.YarnClientImpl: Submitted application application_1494400291896_0002
17/05/10 04:15:49 INFO mapreduce.Job: The url to track the job: http://ip-172-31-1-170.ap-southeast-1.compute.internal:8088/proxy/application_1494400291896_0002/
17/05/10 04:15:49 INFO mapreduce.Job: Running job: job_1494400291896_0002
17/05/10 04:15:56 INFO mapreduce.Job: Job job_1494400291896_0002 running in uber mode : false
17/05/10 04:15:56 INFO mapreduce.Job:  map 0% reduce 0%
17/05/10 04:16:09 INFO mapreduce.Job:  map 5% reduce 0%
17/05/10 04:16:10 INFO mapreduce.Job:  map 10% reduce 0%
17/05/10 04:16:12 INFO mapreduce.Job:  map 13% reduce 0%
17/05/10 04:16:13 INFO mapreduce.Job:  map 15% reduce 0%
17/05/10 04:16:15 INFO mapreduce.Job:  map 17% reduce 0%
17/05/10 04:16:16 INFO mapreduce.Job:  map 19% reduce 0%
17/05/10 04:16:18 INFO mapreduce.Job:  map 20% reduce 0%
17/05/10 04:16:19 INFO mapreduce.Job:  map 21% reduce 0%
17/05/10 04:16:21 INFO mapreduce.Job:  map 22% reduce 0%
17/05/10 04:16:22 INFO mapreduce.Job:  map 23% reduce 0%
17/05/10 04:16:24 INFO mapreduce.Job:  map 25% reduce 0%
17/05/10 04:16:25 INFO mapreduce.Job:  map 26% reduce 0%
17/05/10 04:16:27 INFO mapreduce.Job:  map 27% reduce 0%
17/05/10 04:16:30 INFO mapreduce.Job:  map 28% reduce 0%
17/05/10 04:16:31 INFO mapreduce.Job:  map 29% reduce 0%
17/05/10 04:16:33 INFO mapreduce.Job:  map 30% reduce 0%
17/05/10 04:16:34 INFO mapreduce.Job:  map 32% reduce 0%
17/05/10 04:16:36 INFO mapreduce.Job:  map 34% reduce 0%
17/05/10 04:16:37 INFO mapreduce.Job:  map 36% reduce 0%
17/05/10 04:16:39 INFO mapreduce.Job:  map 37% reduce 0%
17/05/10 04:16:40 INFO mapreduce.Job:  map 38% reduce 0%
17/05/10 04:16:42 INFO mapreduce.Job:  map 39% reduce 0%
17/05/10 04:16:43 INFO mapreduce.Job:  map 40% reduce 0%
17/05/10 04:16:45 INFO mapreduce.Job:  map 41% reduce 0%
17/05/10 04:16:46 INFO mapreduce.Job:  map 42% reduce 0%
17/05/10 04:16:48 INFO mapreduce.Job:  map 43% reduce 0%
17/05/10 04:16:49 INFO mapreduce.Job:  map 44% reduce 0%
17/05/10 04:16:51 INFO mapreduce.Job:  map 46% reduce 0%
17/05/10 04:16:52 INFO mapreduce.Job:  map 47% reduce 0%
17/05/10 04:16:54 INFO mapreduce.Job:  map 48% reduce 0%
17/05/10 04:16:55 INFO mapreduce.Job:  map 49% reduce 0%
17/05/10 04:16:57 INFO mapreduce.Job:  map 51% reduce 0%
17/05/10 04:16:59 INFO mapreduce.Job:  map 52% reduce 0%
17/05/10 04:17:01 INFO mapreduce.Job:  map 54% reduce 0%
17/05/10 04:17:02 INFO mapreduce.Job:  map 55% reduce 0%
17/05/10 04:17:04 INFO mapreduce.Job:  map 56% reduce 0%
17/05/10 04:17:05 INFO mapreduce.Job:  map 58% reduce 0%
17/05/10 04:17:07 INFO mapreduce.Job:  map 59% reduce 0%
17/05/10 04:17:08 INFO mapreduce.Job:  map 61% reduce 0%
17/05/10 04:17:10 INFO mapreduce.Job:  map 62% reduce 0%
17/05/10 04:17:11 INFO mapreduce.Job:  map 63% reduce 0%
17/05/10 04:17:13 INFO mapreduce.Job:  map 65% reduce 0%
17/05/10 04:17:16 INFO mapreduce.Job:  map 67% reduce 0%
17/05/10 04:17:19 INFO mapreduce.Job:  map 69% reduce 0%
17/05/10 04:17:20 INFO mapreduce.Job:  map 70% reduce 0%
17/05/10 04:17:22 INFO mapreduce.Job:  map 71% reduce 0%
17/05/10 04:17:23 INFO mapreduce.Job:  map 72% reduce 0%
17/05/10 04:17:25 INFO mapreduce.Job:  map 73% reduce 0%
17/05/10 04:17:26 INFO mapreduce.Job:  map 74% reduce 0%
17/05/10 04:17:27 INFO mapreduce.Job:  map 75% reduce 0%
17/05/10 04:17:28 INFO mapreduce.Job:  map 76% reduce 0%
17/05/10 04:17:30 INFO mapreduce.Job:  map 77% reduce 0%
17/05/10 04:17:31 INFO mapreduce.Job:  map 78% reduce 0%
17/05/10 04:17:32 INFO mapreduce.Job:  map 79% reduce 0%
17/05/10 04:17:33 INFO mapreduce.Job:  map 80% reduce 0%
17/05/10 04:17:34 INFO mapreduce.Job:  map 81% reduce 0%
17/05/10 04:17:36 INFO mapreduce.Job:  map 82% reduce 0%
17/05/10 04:17:37 INFO mapreduce.Job:  map 83% reduce 0%
17/05/10 04:17:38 INFO mapreduce.Job:  map 84% reduce 0%
17/05/10 04:17:39 INFO mapreduce.Job:  map 85% reduce 0%
17/05/10 04:17:40 INFO mapreduce.Job:  map 86% reduce 0%
17/05/10 04:17:41 INFO mapreduce.Job:  map 87% reduce 0%
17/05/10 04:17:42 INFO mapreduce.Job:  map 88% reduce 0%
17/05/10 04:17:43 INFO mapreduce.Job:  map 89% reduce 0%
17/05/10 04:17:45 INFO mapreduce.Job:  map 91% reduce 0%
17/05/10 04:17:46 INFO mapreduce.Job:  map 92% reduce 0%
17/05/10 04:17:49 INFO mapreduce.Job:  map 94% reduce 0%
17/05/10 04:17:51 INFO mapreduce.Job:  map 95% reduce 0%
17/05/10 04:17:52 INFO mapreduce.Job:  map 96% reduce 0%
17/05/10 04:17:53 INFO mapreduce.Job:  map 97% reduce 0%
17/05/10 04:17:55 INFO mapreduce.Job:  map 98% reduce 0%
17/05/10 04:17:56 INFO mapreduce.Job:  map 99% reduce 0%
17/05/10 04:17:59 INFO mapreduce.Job:  map 100% reduce 0%
17/05/10 04:17:59 INFO mapreduce.Job: Job job_1494400291896_0002 completed successfully
17/05/10 04:17:59 INFO mapreduce.Job: Counters: 31
	File System Counters
		FILE: Number of bytes read=0
		FILE: Number of bytes written=494640
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=344
		HDFS: Number of bytes written=10000000000
		HDFS: Number of read operations=16
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=8
	Job Counters 
		Launched map tasks=4
		Other local map tasks=4
		Total time spent by all maps in occupied slots (ms)=465579
		Total time spent by all reduces in occupied slots (ms)=0
		Total time spent by all map tasks (ms)=465579
		Total vcore-seconds taken by all map tasks=465579
		Total megabyte-seconds taken by all map tasks=476752896
	Map-Reduce Framework
		Map input records=100000000
		Map output records=100000000
		Input split bytes=344
		Spilled Records=0
		Failed Shuffles=0
		Merged Map outputs=0
		GC time elapsed (ms)=1363
		CPU time spent (ms)=152250
		Physical memory (bytes) snapshot=964046848
		Virtual memory (bytes) snapshot=6274400256
		Total committed heap usage (bytes)=868745216
	org.apache.hadoop.examples.terasort.TeraGen$Counters
		CHECKSUM=214760662691937609
	File Input Format Counters 
		Bytes Read=0
	File Output Format Counters 
		Bytes Written=10000000000
    
 ```
 
 Tera sort test
 
 ```
 time hadoop jar /opt/cloudera/parcels/CDH/lib/hadoop-0.20-mapreduce/hadoop-examples.jar terasort /user/shahutsav3988/tg-10GB-4 /user/shahutsav3988/ts-10GB 1>ts_10.out 2>ts_10.err

real	6m19.418s
user	0m10.421s
sys	0m0.566s



17/05/10 04:26:38 INFO terasort.TeraSort: starting
17/05/10 04:26:40 INFO input.FileInputFormat: Total input paths to process : 4
17/05/10 04:26:41 INFO client.RMProxy: Connecting to ResourceManager at ip-172-31-1-170.ap-southeast-1.compute.internal/172.31.1.170:8032
17/05/10 04:26:41 INFO mapreduce.JobSubmitter: number of splits:300
17/05/10 04:26:42 INFO mapreduce.JobSubmitter: Submitting tokens for job: job_1494400291896_0003
17/05/10 04:26:42 INFO impl.YarnClientImpl: Submitted application application_1494400291896_0003
17/05/10 04:26:42 INFO mapreduce.Job: The url to track the job: http://ip-172-31-1-170.ap-southeast-1.compute.internal:8088/proxy/application_1494400291896_0003/
17/05/10 04:26:42 INFO mapreduce.Job: Running job: job_1494400291896_0003
17/05/10 04:26:48 INFO mapreduce.Job: Job job_1494400291896_0003 running in uber mode : false
17/05/10 04:26:48 INFO mapreduce.Job:  map 0% reduce 0%
17/05/10 04:26:57 INFO mapreduce.Job:  map 1% reduce 0%
17/05/10 04:27:00 INFO mapreduce.Job:  map 2% reduce 0%
17/05/10 04:27:02 INFO mapreduce.Job:  map 4% reduce 0%
17/05/10 04:27:08 INFO mapreduce.Job:  map 5% reduce 0%
17/05/10 04:27:11 INFO mapreduce.Job:  map 6% reduce 0%
17/05/10 04:27:14 INFO mapreduce.Job:  map 7% reduce 0%
17/05/10 04:27:15 INFO mapreduce.Job:  map 8% reduce 0%
17/05/10 04:27:20 INFO mapreduce.Job:  map 9% reduce 0%
17/05/10 04:27:21 INFO mapreduce.Job:  map 10% reduce 0%
17/05/10 04:27:29 INFO mapreduce.Job:  map 12% reduce 0%
17/05/10 04:27:31 INFO mapreduce.Job:  map 13% reduce 0%
17/05/10 04:27:35 INFO mapreduce.Job:  map 14% reduce 0%
17/05/10 04:27:41 INFO mapreduce.Job:  map 15% reduce 0%
17/05/10 04:27:42 INFO mapreduce.Job:  map 16% reduce 0%
17/05/10 04:27:43 INFO mapreduce.Job:  map 17% reduce 0%
17/05/10 04:27:45 INFO mapreduce.Job:  map 18% reduce 0%
17/05/10 04:27:52 INFO mapreduce.Job:  map 19% reduce 0%
17/05/10 04:27:53 INFO mapreduce.Job:  map 20% reduce 0%
17/05/10 04:27:55 INFO mapreduce.Job:  map 21% reduce 0%
17/05/10 04:27:59 INFO mapreduce.Job:  map 22% reduce 0%
17/05/10 04:28:02 INFO mapreduce.Job:  map 23% reduce 0%
17/05/10 04:28:06 INFO mapreduce.Job:  map 24% reduce 0%
17/05/10 04:28:07 INFO mapreduce.Job:  map 25% reduce 0%
17/05/10 04:28:08 INFO mapreduce.Job:  map 26% reduce 0%
17/05/10 04:28:14 INFO mapreduce.Job:  map 27% reduce 0%
17/05/10 04:28:15 INFO mapreduce.Job:  map 28% reduce 0%
17/05/10 04:28:20 INFO mapreduce.Job:  map 29% reduce 0%
17/05/10 04:28:21 INFO mapreduce.Job:  map 30% reduce 0%
17/05/10 04:28:25 INFO mapreduce.Job:  map 31% reduce 0%
17/05/10 04:28:28 INFO mapreduce.Job:  map 32% reduce 0%
17/05/10 04:28:31 INFO mapreduce.Job:  map 33% reduce 0%
17/05/10 04:28:33 INFO mapreduce.Job:  map 34% reduce 0%
17/05/10 04:28:36 INFO mapreduce.Job:  map 35% reduce 0%
17/05/10 04:28:38 INFO mapreduce.Job:  map 36% reduce 0%
17/05/10 04:28:44 INFO mapreduce.Job:  map 37% reduce 0%
17/05/10 04:28:45 INFO mapreduce.Job:  map 38% reduce 0%
17/05/10 04:28:46 INFO mapreduce.Job:  map 39% reduce 0%
17/05/10 04:28:51 INFO mapreduce.Job:  map 40% reduce 0%
17/05/10 04:28:55 INFO mapreduce.Job:  map 41% reduce 0%
17/05/10 04:28:57 INFO mapreduce.Job:  map 43% reduce 0%
17/05/10 04:29:02 INFO mapreduce.Job:  map 44% reduce 0%
17/05/10 04:29:06 INFO mapreduce.Job:  map 45% reduce 0%
17/05/10 04:29:08 INFO mapreduce.Job:  map 46% reduce 0%
17/05/10 04:29:09 INFO mapreduce.Job:  map 47% reduce 0%
17/05/10 04:29:13 INFO mapreduce.Job:  map 48% reduce 0%
17/05/10 04:29:17 INFO mapreduce.Job:  map 49% reduce 0%
17/05/10 04:29:20 INFO mapreduce.Job:  map 50% reduce 0%
17/05/10 04:29:22 INFO mapreduce.Job:  map 51% reduce 0%
17/05/10 04:29:25 INFO mapreduce.Job:  map 52% reduce 0%
17/05/10 04:29:28 INFO mapreduce.Job:  map 53% reduce 0%
17/05/10 04:29:31 INFO mapreduce.Job:  map 54% reduce 0%
17/05/10 04:29:35 INFO mapreduce.Job:  map 55% reduce 0%
17/05/10 04:29:36 INFO mapreduce.Job:  map 56% reduce 0%
17/05/10 04:29:38 INFO mapreduce.Job:  map 57% reduce 0%
17/05/10 04:29:42 INFO mapreduce.Job:  map 58% reduce 0%
17/05/10 04:29:46 INFO mapreduce.Job:  map 59% reduce 0%
17/05/10 04:29:48 INFO mapreduce.Job:  map 60% reduce 0%
17/05/10 04:29:49 INFO mapreduce.Job:  map 61% reduce 0%
17/05/10 04:29:52 INFO mapreduce.Job:  map 62% reduce 0%
17/05/10 04:29:57 INFO mapreduce.Job:  map 63% reduce 0%
17/05/10 04:29:59 INFO mapreduce.Job:  map 64% reduce 0%
17/05/10 04:30:02 INFO mapreduce.Job:  map 65% reduce 0%
17/05/10 04:30:04 INFO mapreduce.Job:  map 66% reduce 0%
17/05/10 04:30:07 INFO mapreduce.Job:  map 67% reduce 0%
17/05/10 04:30:10 INFO mapreduce.Job:  map 68% reduce 0%
17/05/10 04:30:13 INFO mapreduce.Job:  map 69% reduce 0%
17/05/10 04:30:15 INFO mapreduce.Job:  map 70% reduce 0%
17/05/10 04:30:18 INFO mapreduce.Job:  map 71% reduce 0%
17/05/10 04:30:20 INFO mapreduce.Job:  map 72% reduce 0%
17/05/10 04:30:26 INFO mapreduce.Job:  map 73% reduce 0%
17/05/10 04:30:27 INFO mapreduce.Job:  map 74% reduce 0%
17/05/10 04:30:29 INFO mapreduce.Job:  map 75% reduce 0%
17/05/10 04:30:33 INFO mapreduce.Job:  map 76% reduce 0%
17/05/10 04:30:36 INFO mapreduce.Job:  map 77% reduce 0%
17/05/10 04:30:39 INFO mapreduce.Job:  map 78% reduce 0%
17/05/10 04:30:40 INFO mapreduce.Job:  map 79% reduce 0%
17/05/10 04:30:43 INFO mapreduce.Job:  map 80% reduce 0%
17/05/10 04:30:47 INFO mapreduce.Job:  map 81% reduce 0%
17/05/10 04:30:51 INFO mapreduce.Job:  map 82% reduce 0%
17/05/10 04:30:52 INFO mapreduce.Job:  map 83% reduce 0%
17/05/10 04:30:53 INFO mapreduce.Job:  map 84% reduce 0%
17/05/10 04:30:59 INFO mapreduce.Job:  map 85% reduce 0%
17/05/10 04:31:05 INFO mapreduce.Job:  map 85% reduce 4%
17/05/10 04:31:06 INFO mapreduce.Job:  map 85% reduce 7%
17/05/10 04:31:07 INFO mapreduce.Job:  map 86% reduce 9%
17/05/10 04:31:08 INFO mapreduce.Job:  map 86% reduce 12%
17/05/10 04:31:09 INFO mapreduce.Job:  map 86% reduce 13%
17/05/10 04:31:11 INFO mapreduce.Job:  map 86% reduce 14%
17/05/10 04:31:12 INFO mapreduce.Job:  map 86% reduce 15%
17/05/10 04:31:13 INFO mapreduce.Job:  map 87% reduce 16%
17/05/10 04:31:14 INFO mapreduce.Job:  map 87% reduce 17%
17/05/10 04:31:19 INFO mapreduce.Job:  map 88% reduce 17%
17/05/10 04:31:20 INFO mapreduce.Job:  map 88% reduce 18%
17/05/10 04:31:23 INFO mapreduce.Job:  map 89% reduce 18%
17/05/10 04:31:27 INFO mapreduce.Job:  map 90% reduce 18%
17/05/10 04:31:31 INFO mapreduce.Job:  map 91% reduce 18%
17/05/10 04:31:37 INFO mapreduce.Job:  map 92% reduce 18%
17/05/10 04:31:41 INFO mapreduce.Job:  map 93% reduce 18%
17/05/10 04:31:44 INFO mapreduce.Job:  map 93% reduce 19%
17/05/10 04:31:45 INFO mapreduce.Job:  map 94% reduce 19%
17/05/10 04:31:50 INFO mapreduce.Job:  map 95% reduce 19%
17/05/10 04:31:55 INFO mapreduce.Job:  map 96% reduce 19%
17/05/10 04:32:00 INFO mapreduce.Job:  map 97% reduce 19%
17/05/10 04:32:03 INFO mapreduce.Job:  map 98% reduce 19%
17/05/10 04:32:06 INFO mapreduce.Job:  map 98% reduce 20%
17/05/10 04:32:08 INFO mapreduce.Job:  map 99% reduce 20%
17/05/10 04:32:12 INFO mapreduce.Job:  map 100% reduce 20%
17/05/10 04:32:14 INFO mapreduce.Job:  map 100% reduce 21%
17/05/10 04:32:15 INFO mapreduce.Job:  map 100% reduce 23%
17/05/10 04:32:17 INFO mapreduce.Job:  map 100% reduce 27%
17/05/10 04:32:18 INFO mapreduce.Job:  map 100% reduce 36%
17/05/10 04:32:20 INFO mapreduce.Job:  map 100% reduce 39%
17/05/10 04:32:21 INFO mapreduce.Job:  map 100% reduce 41%
17/05/10 04:32:22 INFO mapreduce.Job:  map 100% reduce 45%
17/05/10 04:32:23 INFO mapreduce.Job:  map 100% reduce 47%
17/05/10 04:32:24 INFO mapreduce.Job:  map 100% reduce 52%
17/05/10 04:32:26 INFO mapreduce.Job:  map 100% reduce 54%
17/05/10 04:32:27 INFO mapreduce.Job:  map 100% reduce 57%
17/05/10 04:32:28 INFO mapreduce.Job:  map 100% reduce 61%
17/05/10 04:32:29 INFO mapreduce.Job:  map 100% reduce 62%
17/05/10 04:32:30 INFO mapreduce.Job:  map 100% reduce 67%
17/05/10 04:32:31 INFO mapreduce.Job:  map 100% reduce 68%
17/05/10 04:32:32 INFO mapreduce.Job:  map 100% reduce 70%
17/05/10 04:32:33 INFO mapreduce.Job:  map 100% reduce 72%
17/05/10 04:32:34 INFO mapreduce.Job:  map 100% reduce 73%
17/05/10 04:32:36 INFO mapreduce.Job:  map 100% reduce 77%
17/05/10 04:32:37 INFO mapreduce.Job:  map 100% reduce 79%
17/05/10 04:32:38 INFO mapreduce.Job:  map 100% reduce 82%
17/05/10 04:32:39 INFO mapreduce.Job:  map 100% reduce 84%
17/05/10 04:32:40 INFO mapreduce.Job:  map 100% reduce 85%
17/05/10 04:32:41 INFO mapreduce.Job:  map 100% reduce 88%
17/05/10 04:32:42 INFO mapreduce.Job:  map 100% reduce 91%
17/05/10 04:32:43 INFO mapreduce.Job:  map 100% reduce 92%
17/05/10 04:32:45 INFO mapreduce.Job:  map 100% reduce 94%
17/05/10 04:32:47 INFO mapreduce.Job:  map 100% reduce 95%
17/05/10 04:32:48 INFO mapreduce.Job:  map 100% reduce 96%
17/05/10 04:32:50 INFO mapreduce.Job:  map 100% reduce 97%
17/05/10 04:32:51 INFO mapreduce.Job:  map 100% reduce 98%
17/05/10 04:32:53 INFO mapreduce.Job:  map 100% reduce 99%
17/05/10 04:32:56 INFO mapreduce.Job:  map 100% reduce 100%
17/05/10 04:32:56 INFO mapreduce.Job: Job job_1494400291896_0003 completed successfully
17/05/10 04:32:56 INFO mapreduce.Job: Counters: 50
	File System Counters
		FILE: Number of bytes read=4475152592
		FILE: Number of bytes written=8889215633
		FILE: Number of read operations=0
		FILE: Number of large read operations=0
		FILE: Number of write operations=0
		HDFS: Number of bytes read=10000049800
		HDFS: Number of bytes written=10000000000
		HDFS: Number of read operations=930
		HDFS: Number of large read operations=0
		HDFS: Number of write operations=20
	Job Counters 
		Launched map tasks=300
		Launched reduce tasks=10
		Data-local map tasks=299
		Rack-local map tasks=1
		Total time spent by all maps in occupied slots (ms)=2437124
		Total time spent by all reduces in occupied slots (ms)=791890
		Total time spent by all map tasks (ms)=2437124
		Total time spent by all reduce tasks (ms)=791890
		Total vcore-seconds taken by all map tasks=2437124
		Total vcore-seconds taken by all reduce tasks=791890
		Total megabyte-seconds taken by all map tasks=2495614976
		Total megabyte-seconds taken by all reduce tasks=810895360
	Map-Reduce Framework
		Map input records=100000000
		Map output records=100000000
		Map output bytes=10200000000
		Map output materialized bytes=4375245451
		Input split bytes=49800
		Combine input records=0
		Combine output records=0
		Reduce input groups=100000000
		Reduce shuffle bytes=4375245451
		Reduce input records=100000000
		Reduce output records=100000000
		Spilled Records=200000000
		Shuffled Maps =3000
		Failed Shuffles=0
		Merged Map outputs=3000
		GC time elapsed (ms)=36393
		CPU time spent (ms)=1454600
		Physical memory (bytes) snapshot=147487510528
		Virtual memory (bytes) snapshot=485856288768
		Total committed heap usage (bytes)=176405086208
	Shuffle Errors
		BAD_ID=0
		CONNECTION=0
		IO_ERROR=0
		WRONG_LENGTH=0
		WRONG_MAP=0
		WRONG_REDUCE=0
	File Input Format Counters 
		Bytes Read=10000000000
	File Output Format Counters 
		Bytes Written=10000000000
17/05/10 04:32:56 INFO terasort.TeraSort: done
 ```
