List the cloud provider you are using (AWS, GCE, Azure, other)

```
AWS
```

List your instances by their IP address and DNS name

```
172.31.10.8 ip-172-31-10-8.ec2.internal ip-172-31-10-8  - DB 
172.31.2.232 ip-172-31-2-232.ec2.internal ip-172-31-2-232  - CM
172.31.8.89 ip-172-31-8-89.ec2.internal ip-172-31-8-89
172.31.13.182 ip-172-31-13-182.ec2.internal ip-172-31-13-182
172.31.12.71 ip-172-31-12-71.ec2.internal ip-172-31-12-71
```

List the Linux release you are using

```
[ec2-user@ip-172-31-10-8 ~]$ cat /etc/redhat-release 
Red Hat Enterprise Linux Server release 6.9 (Santiago)
```

List the file system capacity for the first node
```
[ec2-user@ip-172-31-10-8 ~]$ lsblk
NAME    MAJ:MIN RM SIZE RO TYPE MOUNTPOINT
xvda    202:0    0  30G  0 disk 
`-xvda1 202:1    0  30G  0 part /

```
List the command and output for yum repolist enabled

```
ec2-user@ip-172-31-10-8 ~]$ yum repolist enabled
Failed to set locale, defaulting to C
Loaded plugins: amazon-id, rhui-lb, search-disabled-repos, security
Repo rhui-REGION-client-config-server-6 forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-client-config-server-6 forced skip_if_unavailable=True due to: /etc/pki/rhui/product/rhui-client-config-server-6.crt
Repo rhui-REGION-client-config-server-6 forced skip_if_unavailable=True due to: /etc/pki/rhui/rhui-client-config-server-6.key
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel6.crt
Repo rhui-REGION-rhel-server-releases forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel6.key
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/cdn.redhat.com-chain.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/product/content-rhel6.crt
Repo rhui-REGION-rhel-server-rh-common forced skip_if_unavailable=True due to: /etc/pki/rhui/content-rhel6.key
Could not contact CDS load balancer rhui2-cds01.us-east-1.aws.ce.redhat.com, trying others.


Could not contact any CDS load balancers: rhui2-cds01.us-east-1.aws.ce.redhat.com, rhui2-cds02.us-east-1.aws.ce.redhat.com.
[ec2-user@ip-172-31-10-8 ~]$ 

```
List the /etc/passwd entries for zhou and chen

 ```
 zhou:x:2800:3100::/home/zhou:/bin/bash
chen:x:2900:3000::/home/chen:/bin/bash


```

List the /etc/group entries for shanghai and beijing
```
shanghai:x:3000:
beijing:x:3100:
```

