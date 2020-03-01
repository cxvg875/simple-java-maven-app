pipeline {
    agent {
		docker{
			image 'maven:3-alpine'
			arges '-v D:/mylib:/root/.m2'
		}
	}
    stages {
        stage('Build') { 
            steps {
                bat 'mvn -B -DskipTests clean package' 
            }
        }
    }
}