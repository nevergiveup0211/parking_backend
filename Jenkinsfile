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
		def mvnHome = tool name: 'Apache Maven 3.6.0', type: 'maven'
    sh "${mvnHome}/bin/mvn -B -DskipTests clean package"
	 }
		}
	
}
}
