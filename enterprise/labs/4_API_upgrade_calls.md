

Report the latest available version of the API
```
curl -u admin:admin 'http://52.221.183.1457180/api/version'
v16
```

Report the CM version
```
curl -u admin:admin 'http://52.221.183.145:7180/api/v16/cm/version'
{
  "version" : "5.11.0",
  "buildUser" : "jenkins",
  "buildTimestamp" : "20170412-1249",
  "gitHash" : "70cb1442626406432a6e7af5bdf206a384ca3f98",
  "snapshot" : false
}

```
List all CM users
```
curl -u admin:admin 'http://52.221.183.145:7180/api/v16/users'
{
  "items" : [ {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ]
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ]
  } ]
}
```
Report the database server in use by CM
```
curl -u admin:admin 'http://52.221.183.145:7180/api/v16/cm/scmDbInfo'
{
  "scmDbType" : "MYSQL",
  "embeddedDbUsed" : false
}
```
