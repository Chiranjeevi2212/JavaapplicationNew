pipeline {
  agent any
  tools {
    maven 'MAVEN_HOME' 
  }
  stages {
    stage ('MyClean') {
      steps {
       'mvn clean'       
      }
    }
    stage ('MyTest') {
      steps {
        bat 'mvn test'
      }
    }    
    stage ('MyPackage') {
      steps {
        bat 'mvn package'
      }
    }   
    stage ('MyInstall') {
      steps {
        bat 'mvn install'
      }
    }   
    stage ('Deploy') {
      steps {
       echo 'Deployed'
      }
    }
      stage ('Success') {
      steps {
       echo 'Pipeline success'
      }
      }    
  }
}
