pipeline {
	agent any 
	stages {
		stage('Build') {
			steps {
				echo "Build"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"
			}
		}
	}
	post {
		always {
			echo 'im super.i run always'
		}
		success {
			echo 'i run when im successful'
		}
		failure {
			echo 'i run when you fail it'
		}
	}
}