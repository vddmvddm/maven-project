
pipeline {
    agent any
    stages{
        stage('Build'){
            steps {
                sh '/etc/apache-maven-3.6.3/bin/mvn clean package'
            }
            post {
                success {
                    echo 'Now Archiving...'
                    archiveArtifacts artifacts: '**/target/*.war'
                }
            }
        }
    }
}
