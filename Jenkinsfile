pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                script {
                  echo 'Building...'
                  bat 'npm install'
                }
            }
        }
    }
}