pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
	     sh 'sudo docker build -t ayushl33t/nodeapp-jenkins:v${BUILD_NUMBER} .' 
            }
        }
	stage('upload artifact'){
	   steps{
		sh 'docker push ayushl33t/nodeapp-jenkins:v${BUILD_NUMBER}'
	   }

	}
    }
}

