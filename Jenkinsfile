pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''date
pwd'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test step'
          }
        }

        stage('Parallel step') {
          steps {
            echo 'parallel step'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}