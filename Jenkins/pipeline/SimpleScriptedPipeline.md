## Simple Scripted Pipeline: 

```
node{
    stage('Build'){
        echo "Inside the build stage"
    }
    stage('Test'){
        echo "Inside the test stage"
    }
    stage('Deploy'){
        echo "Inside the deploy stage"
    }
}
```

## Simple Scripted Pipeline2: 

```dtd
node {
    stage('Preparation') {
        git 'https://github.com/kesharir/jenkins.git'
    }
    stage('Build') {
        bat(/"C:\Program Files\Mvn\apache-maven-3.9.8\bin\mvn" -Dmaven.test.failure.ignore clean test/)
    }
    stage('Package'){
        bat(/"C:\Program Files\Mvn\apache-maven-3.9.8\bin\mvn" -Dmaven.test.failure.ignore clean package/)
    }
    stage('Results') {
        junit '**/target/surefire-reports/TEST-*.xml'
        archiveArtifacts 'target/*.jar'
    }
}


```