


```
[hdfs@ip-172-31-10-8 ec2-user]$ hdfs dfs -ls /user/
Found 8 items
drwxr-xr-x   - chen   chen                0 2017-05-11 23:27 /user/chen
drwxr-xr-x   - hdfs   supergroup          0 2017-05-11 23:25 /user/hdfs
drwxrwxrwx   - mapred hadoop              0 2017-05-11 23:20 /user/history
drwxrwxr-t   - hive   hive                0 2017-05-11 23:21 /user/hive
drwxrwxr-x   - hue    hue                 0 2017-05-11 23:21 /user/hue
drwxrwxr-x   - impala impala              0 2017-05-11 23:21 /user/impala
drwxrwxr-x   - oozie  oozie               0 2017-05-11 23:22 /user/oozie
drwxr-xr-x   - zhou   zhou                0 2017-05-11 23:27 /user/zhou


```

```

[ec2-user@ip-172-31-2-232 ~]$ curl -u admin:admin 'http://54.208.196.38:7180/api/v14/hosts'
{
  "items" : [ {
    "hostId" : "cdad3a66-09eb-4c98-b63d-5b0562f4ad15",
    "ipAddress" : "172.31.10.8",
    "hostname" : "ip-172-31-10-8.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/hostRedirect/cdad3a66-09eb-4c98-b63d-5b0562f4ad15",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15664758784
  }, {
    "hostId" : "6cc295f6-8d47-448b-9862-66e81bbf26bd",
    "ipAddress" : "172.31.12.71",
    "hostname" : "ip-172-31-12-71.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/hostRedirect/6cc295f6-8d47-448b-9862-66e81bbf26bd",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15664758784
  }, {
    "hostId" : "cc603acd-92f9-4db5-bb51-eaf4e7c2d2d2",
    "ipAddress" : "172.31.13.182",
    "hostname" : "ip-172-31-13-182.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/hostRedirect/cc603acd-92f9-4db5-bb51-eaf4e7c2d2d2",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15664758784
  }, {
    "hostId" : "304f62e2-1fa2-41fd-b0fc-5b59238bd9e8",
    "ipAddress" : "172.31.2.232",
    "hostname" : "ip-172-31-2-232.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/hostRedirect/304f62e2-1fa2-41fd-b0fc-5b59238bd9e8",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15664758784
  }, {
    "hostId" : "0ce4f849-000a-4cbc-85a2-ecfa5ad9ae98",
    "ipAddress" : "172.31.8.89",
    "hostname" : "ip-172-31-8-89.ec2.internal",
    "rackId" : "/default",
    "hostUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/hostRedirect/0ce4f849-000a-4cbc-85a2-ecfa5ad9ae98",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "commissionState" : "COMMISSIONED",
    "numCores" : 4,
    "numPhysicalCores" : 2,
    "totalPhysMemBytes" : 15664758784
  } ]
[ec2-user@ip-172-31-2-232 ~]$ 

```

```
[ec2-user@ip-172-31-2-232 ~]$ curl -u admin:admin 'http://54.208.196.38:7180/api/v6/clusters/shahutsav3988/services'
{
  "items" : [ {
    "name" : "hive",
    "type" : "HIVE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/serviceRedirect/hive",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HIVE_HIVEMETASTORES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HIVE_HIVESERVER2S_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hive"
  }, {
    "name" : "zookeeper",
    "type" : "ZOOKEEPER",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/serviceRedirect/zookeeper",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "ZOOKEEPER_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "ZOOKEEPER_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "ZooKeeper"
  }, {
    "name" : "hue",
    "type" : "HUE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/serviceRedirect/hue",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HUE_HUE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Hue"
  }, {
    "name" : "oozie",
    "type" : "OOZIE",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/serviceRedirect/oozie",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "OOZIE_OOZIE_SERVERS_HEALTHY",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Oozie"
  }, {
    "name" : "impala",
    "type" : "IMPALA",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/serviceRedirect/impala",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "IMPALA_ASSIGNMENT_LOCALITY",
      "summary" : "DISABLED"
    }, {
      "name" : "IMPALA_CATALOGSERVER_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "IMPALA_IMPALADS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "IMPALA_STATESTORE_HEALTH",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "Impala"
  }, {
    "name" : "yarn",
    "type" : "YARN",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/serviceRedirect/yarn",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "YARN_JOBHISTORY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_NODE_MANAGERS_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_RESOURCEMANAGERS_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "YARN_USAGE_AGGREGATION_HEALTH",
      "summary" : "DISABLED"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "YARN (MR2 Included)"
  }, {
    "name" : "hdfs",
    "type" : "HDFS",
    "clusterRef" : {
      "clusterName" : "cluster"
    },
    "serviceUrl" : "http://ip-172-31-2-232.ec2.internal:7180/cmf/serviceRedirect/hdfs",
    "serviceState" : "STARTED",
    "healthSummary" : "GOOD",
    "healthChecks" : [ {
      "name" : "HDFS_BLOCKS_WITH_CORRUPT_REPLICAS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_CANARY_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_DATA_NODES_HEALTHY",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_FREE_SPACE_REMAINING",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_HA_NAMENODE_HEALTH",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_MISSING_BLOCKS",
      "summary" : "GOOD"
    }, {
      "name" : "HDFS_UNDER_REPLICATED_BLOCKS",
      "summary" : "GOOD"
    } ],
    "configStalenessStatus" : "FRESH",
    "clientConfigStalenessStatus" : "FRESH",
    "maintenanceMode" : false,
    "maintenanceOwners" : [ ],
    "displayName" : "HDFS"
  } ]
[ec2-user@ip-172-31-2-232 ~]$ 


```
