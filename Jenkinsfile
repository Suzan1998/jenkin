pipeline {
	agent any
	stages{
	

	stage('Integration Test') {
		steps{
		sh 'mvn failsafe:integration-test failsafe:verify'
		}
	}
	
	stage('package') {
		steps{
		sh 'mvn package -DskipTests'
		}
	}
stage('build docker image'){
  steps{
	  script{
		  dockerImage = docker.build("11524920/currency-exchange-devops:${env.BUILD_TAG}")
	  }
  }
}

stage('push docker image'){
	steps{
		script{
			docker.withRegistry('', 'dockerhub')
      dockerImage.push();
	  dockerImage.push('latest');
		}
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
