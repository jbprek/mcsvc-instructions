Build all projects
------------------



Setup
-----
| Service | IP | Ports|URL |
|---------|----|------|----|
|TPP Infrastructure        |
|MariaDB|172.19.0.2| 3306| |
|Gogs   |172.19.0.3| 22 & 3000|http://172.19.0.3:3000|
|Elastic Search   |172.19.0.4| 9300|http://172.19.0.4:9300|
|Infra Services             |
|Eureka1 |172.19.0.10|8761|http://172.19.0.10:8761|
|Zuul TODO|172.19.0.12|-|-|
|Config Service |172.19.0.20|8888|http://172.19.0.20:8888|
|Admin Service|172.19.0.22|9090|http://172.19.0.22:9090|
|Utility Services                                  |
|Constants Service|172.19.0.50|8080|http://172.19.0.50:8080||


Build all projects
------------------
```
mvn clean install -f /home/john/Projects/mcsvc/mcsvc-infra-eureka-service/pom.xml &
mvn clean install -f /home/john/Projects/mcsvc/mcsvc-infra-config-service/pom.xml &
mvn clean install -f /home/john/Projects/mcsvc/mcsvc-infra-admin-service/pom.xml &
mvn clean install -f /home/john/Projects/mcsvc/mcsvc-util-constants-service/pom.xml &
```