pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn clean install -U -DskipTests' 
            }
        }
      stage('Deliver') { 
            steps {
                bat './jenkins/scripts/deliver.sh' 
            }
        }
    }
}
