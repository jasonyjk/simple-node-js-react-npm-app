pipeline {
    agent any

    stages {
        stage('Build') { 
            steps {
                echo "Building in progress."
                sh 'npm install' 
            }
        }
    }

    stage('Test') {
        steps {
            sh './jenkins/scripts/test.sh'
        }
    }
  }
}