pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    echo 'Building...'
                    bat 'echo %PATH%'
                    bat 'npm install'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    echo 'Testing...'
                    bat 'npm test'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo 'Deploying...'
                }
            }
        }
    }
}
