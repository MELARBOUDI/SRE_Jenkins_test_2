pipeline {
  agent any
  stages {
    stage('Stage 1') {
      parallel {
        stage('Stage 1') {
          steps {
            echo 'Hello world!'
          }
        }

        stage('Stage 2') {
          steps {
            sh 'echo \'Hello world!\' '
          }
        }

        stage('Stage 3') {
          steps {
            echo 'Test stage 3 '
          }
        }

      }
    }

    stage('TEST') {
      steps {
        echo 'TEST '
      }
    }

  }
  environment {
    CURRENT_DATE = '${new Date().format(\'yyyyMMddHHmmss\')}'
  }
}