pipeline {
  agent any
    
  tools {nodejs "New"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/paredesjustojp/jpchallenge.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
        sh 'npm rebuild'
      }
    }
     
    stage('deploy') {
      steps {
         sh 'ansible-playbook npm.yml'
      }
    }      
  }
}
