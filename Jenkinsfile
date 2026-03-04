pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/yogesh-kulkarni-DevOps/jenkins-node-app.git'
            }
        }

        stage('Docker Build') {
            steps {
                bat 'docker build -t node-app .'
            }
        }

        stage('Docker Run') {
            steps {
                bat 'docker run -d -p 3000:3000 node-app'
            }
        }

    }
}
