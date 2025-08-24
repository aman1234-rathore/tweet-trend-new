pipeline{
    agent{
        node{
            label 'maven'
        }
    }

    
withEnv(["PATH+MAVEN=/opt/apache-maven-3.9.11/bin"]) {
        sh 'mvn -version'
        // your build steps
    }


    stages{
       stage('build'){
           steps{
               sh 'mvn clen deploy'
    }
}
    }
}




