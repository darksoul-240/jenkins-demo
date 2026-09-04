pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building Python application...'
                bat 'python demo.py'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                bat 'python demo.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                bat 'echo Deployment successful!'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }
    }
}
