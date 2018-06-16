# LearnDW

How to start the LearnDW application from terminal
---

1. Run `mvn clean install` to build your application
1. Start application with `java -jar target/com-learn-dropwizard-1.0-SNAPSHOT.jar server config.yml`
1. To check that your application is running enter url `http://localhost:8080`

How to start the LearnDW application from IDE
---

1. Add new configuration
1. Set Main class = LearnDWApplication
1. Set Program Arguments = server config.yml
1. Save configuration
1. Run or debug from IDE
1. Reference: https://blog.indrek.io/articles/running-a-dropwizard-application-in-intellij-eclipse-and-netbeans/

Health Check
---

To see your applications health enter url `http://localhost:8081/healthcheck`

Endpoints
---
#### Hello World
##### Default request
* http://localhost:8080/hello-world
##### Parameterized request
* http://localhost:8080/hello-world?name=__Your Parameter__

#### Other URLs
All other non implemented endpoints will throw custom 404 error:
* code = 404
* message = Custom page not found error
