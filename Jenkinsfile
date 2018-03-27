pipeline {
  agent any
  stages {
    stage('env') {
      steps {
        sh 'ls -lh '
      }
    }
    stage('pwd') {
      steps {
        sh 'pwd'
      }
    }
    stage('ip') {
      steps {
        sh 'ip addr '
      }
    }
  }
}