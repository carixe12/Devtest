pipeline {
  agent any 

  stages {
    stage('Clone Repository') {
      steps {
        git 'https://git.roky.rocks/roky-team/stalprokat.git'
      }
    }
    
    stage('Install Dependencies') {
      steps {
        sh 'npm install' 
      }
    }
    
    stage('Deploy') {
      steps {
        sh 'npm install -g pm2'
        sh 'pm2 start index.js --name "app"' 
      }
    }
    
    stage('Test') {
      steps {
        sh 'pm2 logs app'
      }
    }
  }
}