## What is SonarQube ? 

- Open Source Code Analysis Tool. 
 SonarQube collects and analyzes source code, measuring quality anf providing reports
  for your projects. 
- Detailed Code Analysis Reports
 SonarQube offers reports on duplicate code, coding standards, unit tests, code coverage,
 code complexity, comments, bugs & security vulnerabilities. 

### Features of SonarQube : 

- Continuos Inspection Of Code
- Centralize Quality Rules 
- Devops Integration
- Enforce Quality Gate
- Dig into issues
- Visualize history of project

### Integrating SonarQube : 

- Create a local project on sonar
- Run on cmd below: 

```
mvn clean verify sonar:sonar 
 -Dsonar.projectKey=Jenkins3 
 -Dsonar.projectName='Jenkins3' 
 -Dsonar.host.url=http://localhost:9000 
 -Dsonar.token=sqp_9536a17b3cb60c3e87d96e0c9a848ed6b0471f3b
```

Note: ProjectKey, ProjectName & Tokens are generated from sonar itself. 

