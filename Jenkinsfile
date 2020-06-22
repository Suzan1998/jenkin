pipeline {
	agent {docker{image 'maven:3.6.3'}}
	stages{
	stage('Build') {
		steps{
		echo 'mvn --version'
		}
	}
	stage('Test') {
		steps{
		echo "Test"
		}
	
	}

	stage('Integration Test') {
		steps{
		echo "Integration Test"
		}
	}
	} 
	post{
		always{
			echo"Iam Suzan"
		}
		success{
			echo"Print when Success"
		}
		failure{
			echo"Print when Fail"
		}
	}

}
