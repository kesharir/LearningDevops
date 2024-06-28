## Simple Scripted Pipeline: 

```
node{
    stage('Build'){
        echo "Inside the build stage"
    }
    stage('Test'){
        ech "Inside the test stage"
    }
    stage('Deploy'){
        echo "Inside the deploy stage"
    }
}
```