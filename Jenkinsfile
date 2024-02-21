pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

        stage('Parallel-Testing') {
          steps {
            echo 'Parallel testing'
          }
        }

      }
    }

  }
}