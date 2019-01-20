pipeline {
  agent any
  stages {
    stage('init') {
      parallel {
        stage('init') {
          steps {
            echo 'this is a min pipeline'
          }
        }
        stage('error') {
          agent any
          steps {
            sh 'echo PATH = ${PATH}'
          }
        }
      }
    }
  }
}