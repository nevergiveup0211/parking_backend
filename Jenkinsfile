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
		
    sh '/opt/apache-maven-3.6.3/bin/mvn -B -DskipTests clean package'
	 }
		}
	
}
}
