pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the repository
                git 'https://github.com/letanloc-tlooc/pypy.git'
            }
        }

        stage('Build') {
            steps {
                // Các bước build (nếu có)
                echo 'Building...'
            }
        }

        stage('Test') {
            steps {
                // Các bước test (nếu có)
                echo 'Testing...'
            }
        }

        stage('Deploy') {
            steps {
                // Các bước deploy (nếu có)
                echo 'Deploying...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
