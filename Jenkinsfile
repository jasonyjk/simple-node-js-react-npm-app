pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
			    echo 'Building in progress.'
                sh 'npm install'
            }
        }
        stage('Test') { 
            steps {
			    echo 'Testing in progress.'
                sh './jenkins/scripts/test.sh' 
            }
        }
    }
}