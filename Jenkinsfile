pipeline {
	agent any
	stages{
	stage('Build') {
		steps{
		echo "$"
		
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
