pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/sagnik-004/capgemini-devops-training'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                bat '''
                if not exist D:\\deploy-demo mkdir D:\\deploy-demo
                copy index.html D:\\deploy-demo
                '''
            }
        }
    }
}