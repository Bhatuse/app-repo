pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Bhatuse/app-repo.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t bhatuse/nginx:latest ./app'
            }
        }
    }
}
