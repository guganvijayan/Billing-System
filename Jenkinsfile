pipeline {
	agent any
	stages{
		stage('compile stage'){
		
		steps{
		withmaven(maven: 'Maven'){
			sh 'mvn clean compile'	
			}
		
		}
	   }	
	stage('Testing stage'){
		
		steps{
		withmaven(maven: 'Maven'){
			sh 'mvn test'	
		}
		
	  }	
	
	}
	
	stage('Deployment stage'){
		
		steps{
		withmaven(maven: 'Maven'){
			sh 'mvn deploy'	
		}
		
	  }	
	
	}	
	
	
	
 }
}