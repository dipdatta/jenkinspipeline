pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Started build'
          }
        }

        stage('Compile') {
          steps {
            echo 'Compilation started'
            emailext(subject: 'Test mail', body: 'this is a test')
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'This is testing'
      }
    }

  }
}