pipeline {
  agent any

  environment {
    APP_NAME = "TYCO APP"
  }

  stages {
    stage('Install') {
      steps { bat 'npm install' }
    }
    stage('Run') {
      steps { 
        bat 'echo %APP_NAME%'
        bat 'npm start' 
      }
    }
  }
}
