pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
	     sh 'docker build -t ayushl33t/nodeapp-jenkins:v${BUILD_NUMBER}' 
            }
        }
    }
}

