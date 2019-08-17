MCSVC Microservices USE
=======================


Environment setup
-----------------
The following enviroment variables are used by docker containers and need to be set
###Eureka IP addreess
``export MCSVC_EUREKA_HOST_1=172.19.0.10``
###Eureka Endpoint
```export MCSVC_EUREKA_HOST_1_URL="http://$MCSVC_EUREKA_HOST_1:8761/eureka"```
###Git repository to be used from config service, pointing to GOGS repo
``export MCSVC_CONFIG_GIT_URL=http://172.19.0.3:3000/mcsvc/mcsvc-infra-config-service-repository.git#``
###Git username
``export MCSVC_CONFIG_GIT_USERNAME=mcsvc``
###Git password
``export MCSVC_CONFIG_GIT_PASSWORD=mcsvc``
###Summary
```
export MCSVC_EUREKA_HOST_1=172.19.0.10
export MCSVC_EUREKA_HOST_1_URL="http://$MCSVC_EUREKA_HOST_1:8761/eureka"
export MCSVC_CONFIG_GIT_URL=http://172.19.0.3:3000/mcsvc/mcsvc-infra-config-service-repository.git
export MCSVC_CONFIG_GIT_USERNAME=mcsvc
export MCSVC_CONFIG_GIT_PASSWORD=mcsvc
```



NETWORK Setup
-------------
Create network 172.19.0.0 mcsvc_net
```
docker network create --subnet 172.19.0.0/16 --gateway  172.19.0.1  mcsvc_net
```


GIT Use - GOGS Initialization
----------------------------
- Step 1 Create Volume for GOGS

```
docker volume create gogs-volume
```

2. Run container create user

`` dada``


2. Import GIT Data from Github repository





