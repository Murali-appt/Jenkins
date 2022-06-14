pipeline {
	// agent any 
	agent { docker { image 'maven:3.6.3'}}
	stages {
		stage('Build') {
			steps {
				sh 'mvn --version'
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