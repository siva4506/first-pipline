pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git 'https://github.com/username/repository.git'
            }
        }
        stage('Code Scan') {
            steps {
                sh 'your-scan-command'
            }
        }
        stage('Build') {
            steps {
                sh 'your-build-command'
            }
        }
        stage('Deploy') {
            steps {
                sh 'docker build -t your_image_name .'
                sh 'docker run -d your_image_name'
            }
        }
    }
}
