# js-serverless-bootstrap
Bootstrap project for all serverless projects written in Node.JS

## One time setup 
* Edit `Serverless.yml` and set `service: <name>-Service`
* Edit `sonar-project.properties` and set 
```
sonar.projectKey=<name>-service
sonar.projectName=<name>-service
```
* Edit `Jenkinsfile` and set `projectName: "<name>-service",`
* Edit config files under `config/environment` and set `CUSTOM_DOMAIN_NAME: "<name>-service.zavasrv.com"`
* Ensure `.env` file with `AWS_SECURITY_GROUP` is created in the root folder to deploy in sandbox. To generate run `create-security-group.sh`

* Ensure _sonarcube_ has the correspponding project created http://sonarqube.svc.zavasrv.com:9000/about (ask Lee Rhodes to create one for you)

* Ensure Jenkins Task is created, clone https://jenkins2.zavasrv.com/job/MakeItFree/job/comms-service/ 


