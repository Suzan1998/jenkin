pipeline {
	agent any
	stages{
	stage('Build') {
		steps{
		echo "Build"
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
			"Print when Success"

		}
		failure{
			echo"Print when Fail"
		}
	}

}
