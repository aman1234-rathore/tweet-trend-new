pipeline {
    agent {
        node{
            label 'maven'
    }
    stages {
        stage('Cloning repo') {
            steps {
                git branch: 'main', url: 'https://github.com/aman1234-rathore/tweet-trend-new.git'
            }
        }
        stage('Build & Test') {
            steps {
                sh 'mvn clean test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'mvn deploy'
            }
        }
    }
}

