pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the repository
                git 'https://github.com/letanloc-tlooc/pypy.git'
            }
        }

        stage('Run demo.py') {
            steps {
                echo 'Running demo1.py...'
                // Chạy file demo.py
                sh 'python3 demo/demo1.py'
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
