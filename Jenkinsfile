pipeline {
    agent {
        node{
            label 'maven'
        }
    }
    
    environment {
        PATH = "/opt/apache-maven-3.9.11/bin:$PATH"
        // Or safer: PATH+MAVEN = "/opt/apache-maven-3.9.11/bin"
    }


    stages {
        stage('Build') {
            steps {
               
                sh 'mvn -version'
                sh 'mvn clean deploy'
                // Add your build steps here
            }
        }
    }
}






