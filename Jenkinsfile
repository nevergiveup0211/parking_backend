pipeline {
   agent any
	stages {
      stage('Git Checkout') {
         steps {
            git 'https://github.com/nevergiveup0211/parking_backend.git'
		}
	}
		stage('Mvn Package') {
         steps {
		def mvnHome= tool name: 'Maven-3', type: 'maven'
		 sh "${mvnHome}/bin/mvn package"
	 }
		}
	
}
}
