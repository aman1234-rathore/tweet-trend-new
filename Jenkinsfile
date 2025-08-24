pipeline {
    agent any

    environment {
        PATH = "/opt/apache-maven-3.9.11/bin:$PATH"
        // Or safer: PATH+MAVEN = "/opt/apache-maven-3.9.11/bin"
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn -version'
                // Add your build steps here
            }
        }
    }
}
