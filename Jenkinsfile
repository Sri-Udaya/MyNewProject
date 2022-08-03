pipeline {
    agent any
    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/Sri-Udaya/MyNewProject.git'
            }
        }
        stage('build WAR') {
	    steps {
		def mvnHome = tool 'maven3'
		bat "${mvnHome}/bin/mvn package"            
	     }
        }
    }
}
