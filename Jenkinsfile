pipeline {
    agent any
    tools {
        maven 'maven3'
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn clean install -U -DskipTests' 
            }
        }
      stage('Deliver') { 
            steps {
                sh './jenkins/scripts/deliver.sh' 
            }
        }
    }
}
