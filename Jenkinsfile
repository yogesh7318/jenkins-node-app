pipeline {
    agent { label 'test-agent' }
    stages {
        stage('Test') {
            steps {
                bat 'echo Running on TEST Agent'
         stage('Docker Build') {
            steps {
                bat 'docker build -t node-app .'
          stage('Docker Run') {
            steps {
                bat 'docker run -d -p 3000:3000 node-app'
  }
}      
  }
}
            }
        }
    }
}
