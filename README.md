# rest-gateway
Act as a single entry application and responsible for dispatching the requests to other micro services
this is the only port which is exposed for public network and accepts requests from outside


# prerequisites
config server should be up and run<br/>
<a href="https://github.com/JavaAdore/config-server">https://github.com/JavaAdore/config-server</a> <br/>
eureka server should be up and run<br/>
<a href="https://github.com/JavaAdore/eureka-server">https://github.com/JavaAdore/eureka-server</a> <br/>


environment variables should be added

# REST_GATEWAY_PORT = 8080
 
# build
as root/Administration <br/>
mvn clean install docker:removeImage docker:build
# run
java -jar target/rest-gateway.jar
