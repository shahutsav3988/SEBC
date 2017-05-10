
Check current state of Hive

```
curl -u admin:admin   'http://localhost:7180/api/v1/clusters/shahutsav3988/services/hive'
{
  "name" : "hive",
  "type" : "HIVE",
  "clusterRef" : {
    "clusterName" : "cluster"
  },
  "serviceUrl" : "http://ip-172-31-1-170.ap-southeast-1.compute.internal:7180/cmf/serviceRedirect/hive",
  "serviceState" : "STARTED",
  "healthSummary" : "GOOD",
  "healthChecks" : [ {
    "name" : "HIVE_HIVEMETASTORES_HEALTHY",
    "summary" : "GOOD"
  }, {
    "name" : "HIVE_HIVESERVER2S_HEALTHY",
    "summary" : "GOOD"
  } ],
  "configStale" : false
```

Stop Hive

```
curl X POST -u admin:admin 'http://localhost:7180/api/v1/clusters/shahutsav3988/services/hive/commands/stop'
{
  "id" : 578,
  "name" : "Stop",
  "startTime" : "2017-05-10T04:40:39.926Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }

```

Start Hive 

```
curl -X POST -u admin:admin 'http://localhost:7180/api/v1/clusters/shahutsav3988/services/hive/commands/start'
{
  "id" : 582,
  "name" : "Start",
  "startTime" : "2017-05-10T04:41:26.254Z",
  "active" : true,
  "serviceRef" : {
    "clusterName" : "cluster",
    "serviceName" : "hive"
  }

```
