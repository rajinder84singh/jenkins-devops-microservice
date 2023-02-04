pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo "Build"
				echo "$PATH"
				echo "Build ID - $env.BUILD_ID"
				echo "Build No - $env.BUILD_NO"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
		}
		stage('IntegrationTest') {
			steps {
				echo "IntegrationTest"
			}			
		}
	} 

	post {
		always {
			echo 'I run always'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I run when you failure'
		}
	}
}
