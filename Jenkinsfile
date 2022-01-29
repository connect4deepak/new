pipeline {
  agent any
  stages {
    stage('staging') {
      steps {
        sh 'pwd'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'this is me'
          }
        }

        stage('newtest') {
          steps {
            echo 'me'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sh '''pwd
date'''
        echo 'shoe result'
      }
    }

  }
}