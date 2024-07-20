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
		stage('Deliver') { 
            steps {
			    echo 'Deliver in progress.'
                sh './jenkins/scripts/deliver.sh' 
                input message: 'Finished using the web site? (Click "Proceed" to continue)' 
                sh './jenkins/scripts/kill.sh' 
            }
        }
    }
}