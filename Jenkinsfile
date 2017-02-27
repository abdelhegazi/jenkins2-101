node {
  //  agent any
        stage('Build') {
                echo 'Building..'
		git url: 'https://github.com/jglick/simple-maven-project-with-tests.git'
        }
        stage('Test') {
                echo 'Testing..'
		def mvnHome = tool 'M3'
		/bin/bash "${mvnHome}/bin/mvn -B verify"
        }
        stage('Deploy') {
                echo "${mvnHome}"
        }
}
