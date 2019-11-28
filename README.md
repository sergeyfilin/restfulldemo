```
mvn verify sonar:sonar 
```
```
mvn clean package && java -javaagent:target/jacoco-agent/org.jacoco.agent-runtime.jar=append=true,includes=*,output=file,destfile=target/jacoco-report/jacoco.exec -jar ./target/code-coverage-0.1.0.jar
```

```
mvn -Dsonar.coverage.jacoco.xmlReportPaths=jacoco.xml sonar:sonar 
```