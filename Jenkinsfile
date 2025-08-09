pipeline{
    agent {
        node{
            label 'maven'
        }
    }
    
    stages{
        stage('Clone code on slave system'){
            steps{
                git url: 'https://github.com/aman1234-rathore/tweet-trend-new.git', branch: 'main'
            }
        }
        stage('build'){
            steps{
                sh 'mvn clen deploy'
            }
        }
    }
}