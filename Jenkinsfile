
pipeline {
    agent any
    tools {
        jdk 'JDK17' // Make sure you have JDK17 configured in Jenkins Global Tools
    }
    stages {
        stage('Build') {
            steps {
                sh 'java -version'
                sh 'mvn clean deploy'
            }
        }
    }
}