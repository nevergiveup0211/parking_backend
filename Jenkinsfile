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
		def mvn = tool (name: 'maven3', type: 'maven') + '/bin/mvn'
		 sh "${mvn} clean package deploy"
	 }
		}
	
}
}
