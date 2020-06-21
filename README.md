# java-wiremock-server
An implementation of Wiremock running on a servlet container (Tomcat)

Note 1: In order to access tomcat manager a new user needs to be created. 
```
<role rolename="manager-gui"/>
<user username="admin" password="admin" roles="manager-gui"/>
```

#### Features 
- API mocking 
 
## 

## Application Stack

Stack  | version |
--- | --- |  
*Java* | 1.8 
*Frontend* | n/a 
*Server* | Tomcat (External)
*Build Tool* | Gradle
*CI* | n/a  
*Code Coverage* | n/a
*Build env* | local tomcat .war

## Application Build
gradle :war

## Application Run

```
> Build, Execution, Deployment > Build Tools > Gradle
Build and run using : Intellij IDEA
```

```
Tomcat Server > local

    Server: 
        HTTP port: 8082
    Deployments:
        wiremock-server.war (exploded)
        Application Context: /wiremock
```
 
## Application URL
- http://localhost:8082/wiremock/api/mytest
- http://localhost:8082/manager/html (admin/admin)
