pipeline {
  agent any
    
  tools {nodejs "NodeJS"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/nurlan1407/sre7.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh 'npm start'
      }
    }  
    
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}
