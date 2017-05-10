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
 
 
