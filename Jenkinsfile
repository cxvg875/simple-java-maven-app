pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo '1123'
      }
    }

    stage('TEST') {
      parallel {
        stage('TEST') {
          steps {
            echo 'test'
          }
        }

        stage('report') {
          steps {
            echo 'report'
          }
        }

      }
    }

  }
  environment {
    VAR1 = '1'
  }
}