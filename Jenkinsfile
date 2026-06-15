pipeline {
	agent any
	 
	 tools {
	 	gradle 'Gradle'
	 }
	 
	 stages {
	 	
	 	stage('Check-out') {
	 		steps {
	 			git branch :'main' , url :'https://github.com/ChallaPraneeth26/gradlepipeline'
	 		}
	 	}
	 	
	 	stage('Build') {
	 		steps {
	 			
	 				sh 'gradle build'
	 			
	 		}
	 	}
	 	
	 	stage('Run application') {
	 		steps {
	 			
	 				sh 'gradle run'
	 			
	 		}
	 	}
	 	
	 	}
	 	post {
	 		success {
	 			echo 'Gralde Ec=xecuted succesfully'
	 		}
	 		failure {
	 			echo 'Gradle not executed'
	 		}	
	 	}
	 }
	 	
