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
        echo 'go to your ansible server and execute ansible-playbook npm.yml'
      }
    }      
  }
}
