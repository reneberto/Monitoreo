


$ mkdir tig-stack
$ cd tig-stack
$ curl -OL https://raw.githubusercontent.com/matisku/tig-stack/master/docker-compose.yml
$ docker-compose up -d
```

## Environment
### Grafana  
`GF_INSTALL_PLUGINS` - In default all plugins are installed  
`GF_SECURITY_ADMIN_USER` - Admin Username. Default: `admin`  
`GF_SECURITY_ADMIN_PASSWORD`- Admin User Password. Default:`admin`  
`GF_SECURITY_SECRET_KEY` - Secret key. Default: `grafana`  
`GF_USERS_ALLOW_SIGN_UP` - Allow singup to Grafana. Default: `"true"`  
`GF_USERS_ALLOW_ORG_CREATE` - Allow user create new Orgs. Default: `"true"`  
`GF_AUTH_ANONYMOUS_ENABLED` - Anonymus autthorization enabled. Default: `"true"`  
`GF_AUTH_ANONYMOUS_ORG_NAME` - Anonymus defaul Org Name. Default: `grafana`   
`GF_DASHBOARDS_JSON_ENABLED` - Dashboards as JSON enabled. Default: `"true"`   
`GF_DASHBOARDS_JSON_PATH` - Path where JSON Dashboards are stored. Default: `/opt/grafana`   

### InfluxDB  
`INFLUX_DATABASE` - IndluxDB Database Name. Default:  `"telegraf"`   
`INLFUX_ADMIN_USER` - IndluxDB Admin Username. Default: `"grafana"`  
`INFLUX_ADMIN_PASS` - InfluxDB Admin Password. Default: `"grafana"`    

### Telegraf  
`HOST_NAME` - Telegraf Default Hostane. Default: `"telegraf"`  
`INFLUXDB_HOST` - IndluxDB Database Host. Default: `"influxdb"`  
`INFLUXDB_PORT` - InfluxDB Default Port. Default: `"8086"`  
`DATABASE` - InfluxDB Database where telegraf stores data. Default: `"telegraf"`  

## Ports
Grafana: `3000`
InfluxDB: `8083`, `8086`
## JVM use Jolokia https://jolokia.org/

