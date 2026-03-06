pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/ahs0042/fastapi-devops-app.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t ahs0042/fastapi-app:latest .'
            }
        }
    }
}
