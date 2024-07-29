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
      post {
       success {
        echo "build succeeded :)"
       }
       failure {
        echo "build failed :("
       }
      }
    }
}
