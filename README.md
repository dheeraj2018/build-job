jenkins jobs
pipeline {
 agent any
 
  stages {
   stage('Build') {
   steps {
     echo 'Buliding..'
    }
   }
   stage('deploy') {
   steps {
    echo 'deploying..'
    }
   }
   stages('test') {
   steps {
    echo 'testing..'
    }
   }
  }
 }
