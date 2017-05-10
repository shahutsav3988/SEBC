1. What is ubertask optimization?

```
Ubertask Maximum Maps
mapreduce.job.ubertask.maxmaps

Threshold for number of maps, beyond which job is considered too big for the ubertasking optimization. Users may override this value, but only downward.
```

2. Where in CM is the Kerberos Security Realm value displayed?

```
Administration > Settings > Kerberos > Kerberos Security Realm
```

3. Which CDH service(s) host a property for enabling Kerberos authentication?

```
Administration > Security
```

4. How do you upgrade the CM agents?
```
1. Stop Cloudera Manager Server, Database(if embedded), and Agent

2. Upgrade Cloudera Manager Server (Packages)

3. Replace the repo file in the configuration location for the package management software

4. 
sudo yum clean all $ sudo yum upgrade cloudera-manager-server cloudera-manager-daemons cloudera-manager-server-db-2 cloudera-manager-agent

5. Start services again
```

5. Give the tsquery statement used to chart Hue's CPU utilization?

```
SELECT cpu_system_rate
WHERE 
 roleType=HUE_SERVER
```

6. Name all the roles that make up the Hive service

```
Hive Metastore Server
HiveServer2
Hive Gateway
```

7. What steps must be completed before integrating Cloudera Manager with Kerberos?

```
1 Install Packages on KDC server  - krb5-server , krb5-libs , krb5-auth-dialog-workstation
2 Install Packages on KDC client  - krb5-workstation ,krb5-libs , krb5-auth-dialog-workstation

3 Kdc.conf -set realm name - <abc.com>,  max life 1day =1d, mex renewable life 7day = 7day

4 update krb5.conf 
default realm name - same as kdc.conf
renew same as kdc.conf
[realms]
realm name
kdc = hostname
admin_server = hostname

[domain_realm]
.only last part of hostname=realm name
only last part of hostname=realm name

5 Create DB for KDC server 

6 add principal for cloudera manager to enable kerberos

7 Add in ACL 

8 Add policies

addpol admin
addpol users
addpol hosts

9 start krb server 

service krb5kdc start
service kadmin start

10 krb5.conf copy to all client machines 

11 login to CM - Cloudera Manager

Go to Administation 
 Security 
 Enable kerberos and follow rest of steps on CM.
 ```
