pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/Sri-Udaya/MyNewProject.git'
            }
        }
        stage('build WAR') {
	    environment {
		 mvnHome = tool 'maven3'
	    }
	    steps {
		bat "${env.mvnHome}/bin/mvn package"            
	     }
        }
    }
}
