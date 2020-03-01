pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
    }

  }
  stages {
    stage('build') {
      steps {
        echo '1123'
        sh 'npm install'
        timeout(time: 10, activity: true) {
          sleep 5
          build(job: 'test', propagate: true, wait: true, quietPeriod: 3)
        }

      }
    }

  }
  environment {
    VAR1 = '1'
  }
}