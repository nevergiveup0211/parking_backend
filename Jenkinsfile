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
		bat label: '', script: 'mvn clean package deploy'
	 }
		}
	
}
}
