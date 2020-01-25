# spring-cloud-config
Example for a spring cloud config client/server. 
See also: 
- https://www.baeldung.com/spring-cloud-configuration
- https://cloud.spring.io/spring-cloud-config/multi/multi__spring_cloud_config_server.html

## Config-Server test
So we can retrieve the configuration for our planned config client running under development profile in branch master via:
curl http://root:s3cr3t@localhost:8888/config-client/development/master

## Config-Client test
To test, if the configuration is properly received from our server and the role value gets injected in our controller method, we simply curl it after booting the client:
curl http://localhost:8080/whoami/Mr_Pink

