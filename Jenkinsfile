pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'echo \'Building\''
      }
    }

    stage('Test') {
      parallel {
        stage('Api Test') {
          steps {
            echo 'echo \'Testing\''
          }
        }

        stage('Unit Test') {
          steps {
            echo 'Api Testing'
          }
        }

      }
    }

    stage('Archive') {
      steps {
        echo 'echo \'Archiving\''
      }
    }

  }
}