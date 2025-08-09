pipeline {
    agent any

    environment {
        JAVA_HOME = "/usr/lib/jvm/java-17-openjdk-amd64"
        PATH = "${JAVA_HOME}/bin:${env.PATH}"
    }

    stages {
        stage('Install Java 17') {
            steps {
                sh '''
                    echo "Installing Java 17 if not already present..."
                    if ! java -version 2>&1 | grep -q "17."; then
                        sudo apt-get update -y
                        sudo apt-get install -y openjdk-17-jdk
                    fi
                    java -version
                '''
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}