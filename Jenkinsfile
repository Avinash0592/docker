
pipeline{

	agent any

	environment {
		DOCKERHUB_CREDENTIALS=credentials('DokcerID')
	}
stages {

		stage('Build') {

			steps {
				sh 'docker build -t avinashsanam/python:2.7-slim .'
			}
		}
  stage('Push') {

			steps {
				sh 'docker push avinashsanam/python:2.7-slim'
			}
		}
}
}
