pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'g++ src/main.cpp -o app.exe'
            }
        }

        stage('Test') {
            steps {
                bat 'test\\run-tests.bat'
            }
        }

        stage('Deploy') {
            steps {
                bat 'deploy.bat'
            }
        }
    }
}
