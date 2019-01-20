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
        stage('') {
          agent {
            docker {
              image 'maven:3.3.9-jdk-8'
            }

          }
          steps {
            sh 'echo PATH = ${PATH}'
          }
        }
      }
    }
  }
}