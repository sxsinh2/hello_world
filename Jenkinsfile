library 'SharedLibs'


pipeline {
  agent {
    docker {
      image 'maven:alpine'
    }
    
  }
  stages {
    stage('Step1') {
      steps {
        sh 'mvn -v'
      }
    }
    stage('Shared Lib') {
         steps {
             helloWorld("Jenkins")
         }
      }
  }
}
