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
		    bat './jenkins/scripts/test.sh'
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
