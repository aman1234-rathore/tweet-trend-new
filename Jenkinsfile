pipeline {
    agent {
        node{
            label 'maven'
        }
    }

    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/aman1234-rathore/tweet-trend-new.git'
                sh 'mvn -version'
                sh 'mvn clean deploy'
                // Add your build steps here
            }
        }
    }
}





