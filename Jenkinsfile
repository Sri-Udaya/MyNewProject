pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/Sri-Udaya/MyNewProject.git'
            }
        }
        stage('build WAR') {
	    script {
		def mvnHome = tool 'maven3'
	    }
	    steps {
		bat "${mvnHome}/bin/mvn package"            
	     }
        }
    }
}
