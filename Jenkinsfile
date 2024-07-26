pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                bat 'mvn clean install -U -DskipTests' 
            }
        }
      stage('Deliver') { 
            steps {
                bat './jenkins/scripts/deliver.sh' 
            }
        }
    }
}
