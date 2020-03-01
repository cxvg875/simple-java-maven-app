pipeline {
    agent {
		docker{
			image 'maven:3-alpine'
			args '-v D:/mylib:/root/.m2'
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