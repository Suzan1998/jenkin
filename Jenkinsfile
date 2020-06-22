pipeline {
	agent any

	environment{
		dockerHome = tool 'myDocker'
		maneHome = tool 'myMaven'
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH" 
	}
	stages{
	stage('Build') {
		steps{
			sh 'mvn --version'
			sh 'docker version'
		echo "$PATH"
		
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
