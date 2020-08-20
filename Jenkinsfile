//Scripted 

//Declarative
pipeline {
	agent any 
	//agent { docker { image 'maven:3.6.3' } }
	//agent { docker { image 'node:13.8' } }
	stages {
		stage ('Build'){
			steps {
				//sh "mvn --version"
				//sh "node --version"
				echo "Build"
				echo "Job '${JOB_NAME}' (${BUILD_NUMBER}) is waiting for input"
			}
		}
		stage ('Unit test'){
			steps {
				echo "Unit test"
			}
		}
		stage ('Integration test'){
			steps {
				echo "Integration test"
			}
		}
	} 
	post {
		always {
			echo "I'm awesome. I run always"
		}
		success {
			echo "I run when you are successful"
		}
		failure {
			echo "I run when you fail"
		}
	}

}
