
```
curl -u admin:admin 'http://52.221.183.1457180/api/v2/cm/deployment'
{
  "timestamp" : "2017-05-10T07:28:53.017Z",
  "clusters" : [ {
    "name" : "shahutsav3988",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "443547648"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "443547648"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "912680550"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "153"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-1-170.ap-southeast-1.compute.internal"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "hive_password"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-57ddac191f21438b5b430da38cac9c9c",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-08a5fb86fa25548b3"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-6409c46045ed107108ad8316001b9acf",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-00d56e0daa205f9f3"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-d40b0b4a06a602207335d290de4f1267",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "i-0dab79db9527dd9cb"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9phd9ujktitrl6qp9knejtke9"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7h2s6jce4hzd1qe67rkfjnh2g"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "443547648"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a4s025u2kyet7l9sj8743jm4l"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-57ddac191f21438b5b430da38cac9c9c",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-08a5fb86fa25548b3"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "520ca5a4hz4yqpd33pwit3px6"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-d40b0b4a06a602207335d290de4f1267",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "i-0dab79db9527dd9cb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4i804k3nzd4oac8bpnrau50g9"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-1-170.ap-southeast-1.compute.internal"
        }, {
          "name" : "database_password",
          "value" : "hue_password"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-2d4c5ed427cad5af326d47dcbfeb3cdd"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "c618vfdea3gvtcxbzqj1n835j"
          }, {
            "name" : "secret_key",
            "value" : "gekwoswFg2njt9uZW4oUIRYcebiFij"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-1-170.ap-southeast-1.compute.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "oozie_password"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "443547648"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ckkm9ttle9p0zzslbil0u2f3k"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "10"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "443547648"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "5192"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "443547648"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "5192"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "3"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "80"
        }, {
          "name" : "yarn_service_cgroups",
          "value" : "false"
        }, {
          "name" : "yarn_service_lce_always",
          "value" : "false"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "OE8GT40HcVza7brDviusgDdzFb1UDb"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "897fnowbhr9ref06afwfshr41"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "gtfoqxb3qcaxd5ukt2b58x50"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-57ddac191f21438b5b430da38cac9c9c",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-08a5fb86fa25548b3"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8prta5fyhe5nue3ud0m9n4s6j"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-6409c46045ed107108ad8316001b9acf",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-00d56e0daa205f9f3"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a3bhdeihyr1sjuh1vradv2sn9"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-d40b0b4a06a602207335d290de4f1267",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "i-0dab79db9527dd9cb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "a8kx6ehhuhyl4wse5ahykzlqk"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "64"
          }, {
            "name" : "role_jceks_password",
            "value" : "8cee9hu99kll5l5ynse1r1laq"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "443547648"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "datanode_java_heapsize",
            "value" : "1073741824"
          }, {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "3157155020"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4294967296"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_handler_count",
            "value" : "32"
          }, {
            "name" : "dfs_namenode_service_handler_count",
            "value" : "32"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "dfs_safemode_min_datanodes",
            "value" : "0"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "1073741824"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "bEj4O2PDlpmrCrQWmXzvHWDD3uzmsZ"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "oYv7DdUW3eBnV5KQZyNpET7DcIiTAc"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "2Z5aZQY0AveS39Mu8hk4Ug2Yxqz8Vv"
        }, {
          "name" : "rm_dirty",
          "value" : "false"
        }, {
          "name" : "rm_last_allocation_percentage",
          "value" : "20"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7545tfmf5kb76795ehqigcmc3"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-57ddac191f21438b5b430da38cac9c9c",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-08a5fb86fa25548b3"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8nugqisaz07cmcuhntl0afc4m"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-6409c46045ed107108ad8316001b9acf",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-00d56e0daa205f9f3"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4znr03c7knmyvb2wywv04mnqr"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-d40b0b4a06a602207335d290de4f1267",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "i-0dab79db9527dd9cb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "43gmef6nutcn6k5yf1ty1m45k"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-2d4c5ed427cad5af326d47dcbfeb3cdd",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "i-033c04b64ce766271"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "66"
          }, {
            "name" : "role_jceks_password",
            "value" : "8yy1acopuc7nhgn9182tfvju4"
          } ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-d40b0b4a06a602207335d290de4f1267",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "i-0dab79db9527dd9cb"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1dx27lxjqqobgyelj7ng9r2bz"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "i-033c04b64ce766271",
    "ipAddress" : "172.31.1.170",
    "hostname" : "ip-172-31-1-170.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0dab79db9527dd9cb",
    "ipAddress" : "172.31.17.196",
    "hostname" : "ip-172-31-17-196.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-08a5fb86fa25548b3",
    "ipAddress" : "172.31.20.5",
    "hostname" : "ip-172-31-20-5.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-00d56e0daa205f9f3",
    "ipAddress" : "172.31.27.79",
    "hostname" : "ip-172-31-27-79.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "i-0e04f5a98d85bff02",
    "ipAddress" : "172.31.29.239",
    "hostname" : "ip-172-31-29-239.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-ACTIVITYMONITOR-2d4c5ed427cad5af326d47dcbfeb3cdd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c7acbddcb3a0ca7bdada39faa0fb229be7e9fa87ba77125ab6819f4e0a613ee7",
    "pwSalt" : 8716898980324239695,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-2d4c5ed427cad5af326d47dcbfeb3cdd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "f2e6ab3f62a0496a76097ef9c40196c417b02b788c9bc10daf241e269892c2ec",
    "pwSalt" : 2132327364465284363,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-2d4c5ed427cad5af326d47dcbfeb3cdd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "baab75b6af5e5aa46471f1907ad7587ddadf31451c49b04c23bbcde3e11bf29d",
    "pwSalt" : -6021204303969139521,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-2d4c5ed427cad5af326d47dcbfeb3cdd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "350f4d7878a255311ccf5ad9d8597bfa31f6763b0f9542f2e0c00f3148b20fd0",
    "pwSalt" : 7678369072626216211,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-2d4c5ed427cad5af326d47dcbfeb3cdd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "16bd2f3dbcde31927a284ec8fcf5fd2c2aa1a56413852774ff3746e13e338f01",
    "pwSalt" : 6268014968422589037,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "5d9b4ebc55a8c3a278d4f31e95da5879e1f22164777f6303203be998ff0794f4",
    "pwSalt" : -4653228628926814131,
    "pwLogin" : true
  }, {
    "name" : "minotaur",
    "roles" : [ "ROLE_CONFIGURATOR" ],
    "pwHash" : "9fab50c81a807f3972a35dad3c011b9e1d1938486ee6d597ca94cb330ce5281b",
    "pwSalt" : 3558478561091245113,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.11.0",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170412-1249",
    "gitHash" : "70cb1442626406432a6e7af5bdf206a384ca3f98",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "ACTIVITYMONITOR",
        "items" : [ {
          "name" : "firehose_database_host",
          "value" : "ip-172-31-1-170.ap-southeast-1.compute.internal"
        }, {
          "name" : "firehose_database_name",
          "value" : "amon"
        }, {
          "name" : "firehose_database_password",
          "value" : "amon_password"
        }, {
          "name" : "firehose_database_user",
          "value" : "amon"
        }, {
          "name" : "firehose_heapsize",
          "value" : "443547648"
        } ]
      }, {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "443547648"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-1-170.ap-southeast-1.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "rman_password"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "443547648"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-2d4c5ed427cad5af326d47dcbfeb3cdd",
      "type" : "ACTIVITYMONITOR",
      "hostRef" : {
        "hostId" : "i-033c04b64ce766271"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "9djpwxuztqbaz8zo3j4v75n9w"
        } ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-2d4c5ed427cad5af326d47dcbfeb3cdd",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "i-033c04b64ce766271"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "c2q00bplprf37z0wb2xpg6ede"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-2d4c5ed427cad5af326d47dcbfeb3cdd",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "i-033c04b64ce766271"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "1a1jhpiu7vx3ttxlt3i54nx4i"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-2d4c5ed427cad5af326d47dcbfeb3cdd",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "i-033c04b64ce766271"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ijhs7x6dz3t9y75h7wsdd90z"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-2d4c5ed427cad5af326d47dcbfeb3cdd",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "i-033c04b64ce766271"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "19g3n90p1kmd9hqej055c6s92"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-2d4c5ed427cad5af326d47dcbfeb3cdd",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "i-033c04b64ce766271"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "4r5m6354dbejhpdt03uzxn03b"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/27/2012 5:50"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/"
    } ]
  }
}
```
