pipeline {
	agent any
	
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/swapnil/Documents/GRRAS/apache-maven-3.6.0/bin/mvn install'
	                 }}
		stage('Deployment'){
		    steps {
			
			sh 'cp target/LoginWebApp.war swapnil@127.0.1.1:/home/swapnil/Documents/GRRAS/apache-tomcat-8.5.35/webapps'
	}
}}}
