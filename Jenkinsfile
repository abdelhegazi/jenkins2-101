
pipeline {
    agent any

      stages {

        stage('Build') {
	   steps {
                echo 'Building ...'
		git url: 'https://github.com/jglick/simple-maven-project-with-tests.git'
           }
	} 

        stage('Test') {
	    steps {	
                echo 'Testing ...'
//		def mvnHome = tool 'M3'
//		/bin/bash "${mvnHome}/bin/mvn -B verify"
            }
	}
	
	stage('Integration Test') {
		steps {
			echo "integration test"
		}
	}

	stage('Static Analysis') {
		steps {
			echo 'Static Analysis'
		}
	}

        stage('Deploy') {
	    steps {
//                echo "${mvnHome}"
		echo 'Deploying ...'
            }
	}
    }
}
