Check vm.swappiness on all your nodes
```
cat /proc/sys/vm/swappiness
1

echo 1 > /proc/sys/vm/swappiness
```
Show the mount attributes of your volume(s)

```
mount
/dev/xvda1 on / type ext4 (rw)
proc on /proc type proc (rw)
sysfs on /sys type sysfs (rw)
devpts on /dev/pts type devpts (rw,gid=5,mode=620)
tmpfs on /dev/shm type tmpfs (rw,rootcontext="system_u:object_r:tmpfs_t:s0")
none on /proc/sys/fs/binfmt_misc type binfmt_misc (rw)
cm_processes on /var/run/cloudera-scm-agent/process type tmpfs (rw,mode=0751,rootcontext="unconfined_u:object_r:var_run_t:s0")
cm_cgroups on /var/run/cloudera-scm-agent/cgroups/blkio type cgroup (rw,blkio)
cm_cgroups on /var/run/cloudera-scm-agent/cgroups/cpuacct type cgroup (rw,cpuacct)
cm_cgroups on /var/run/cloudera-scm-agent/cgroups/cpu type cgroup (rw,cpu)
cm_cgroups on /var/run/cloudera-scm-agent/cgroups/memory type cgroup (rw,memory)

```

Disable transparent hugepage support

```
echo 'never' > /sys/kernel/mm/redhat_transparent_hugepage/defrag
echo 'never' > /sys/kernel/mm/redhat_transparent_hugepage/enabled
```
List your network interface configuration
```
ifconfig
eth0      Link encap:Ethernet  HWaddr 02:29:A0:80:09:7F  
          inet addr:172.31.1.170  Bcast:172.31.15.255  Mask:255.255.240.0
          inet6 addr: fe80::29:a0ff:fe80:97f/64 Scope:Link
          UP BROADCAST RUNNING MULTICAST  MTU:9001  Metric:1
          RX packets:9215240 errors:0 dropped:0 overruns:0 frame:0
          TX packets:3847426 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:1000 
          RX bytes:28759881373 (26.7 GiB)  TX bytes:16736637815 (15.5 GiB)
          Interrupt:145 

lo        Link encap:Local Loopback  
          inet addr:127.0.0.1  Mask:255.0.0.0
          inet6 addr: ::1/128 Scope:Host
          UP LOOPBACK RUNNING  MTU:65536  Metric:1
          RX packets:7358411 errors:0 dropped:0 overruns:0 frame:0
          TX packets:7358411 errors:0 dropped:0 overruns:0 carrier:0
          collisions:0 txqueuelen:0 
          RX bytes:14085154925 (13.1 GiB)  TX bytes:14085154925 (13.1 GiB)
```

Show that forward and reverse host lookups are correctly resolved
For /etc/hosts, use getent
For DNS, use nslookup


Show the nscd service is running
```
service nscd status
nscd (pid 3062) is running...

```

Show the ntpd service is running

```
service ntpd status
ntpd (pid  3119) is running...

```

