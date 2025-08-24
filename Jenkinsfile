pipeline{
    agent{
        node{
            label 'maven'
        }
    }
    withEnv(["PATH+MAVEN=/opt/apache-maven-3.9.11/bin"]){
        PATH = '/opt/apache-maven-3.9.11/bin:$PATH'
    }
    stages{
       stage('build'){
           steps{
               sh 'mvn clen deploy'
    }
}
    }
}



