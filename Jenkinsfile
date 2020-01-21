
pipeline {
    agent any
 
 tools {
        maven 'localMaven'
    }
 
    stages{
        steps('Build'){
            sh 'mvn clean package'
        }
    }
}
