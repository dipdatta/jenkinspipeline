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