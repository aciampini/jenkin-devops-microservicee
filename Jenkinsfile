//SCRIPTED
//DECLARATIVE
pipeline {
	// agent any
	//agent { docker { image 'maven:3.9.8' } }
	agent { docker { image 'node:13.8' } }
	stages {
		stage('Build') {
			steps {
				//echo 'mvn --version'
				echo 'node --version'
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
			echo 'Im awesome. I run always'
		}
		success {
			echo 'I run when you are succesful'
		}
		failure {
			echo 'I run when you fail'
		}
	}
}