pipeline {
  agent any
  stages {
    stage('env_info') {
      parallel {
        stage('env') {
          steps {
            sh 'env'
          }
        }
        stage('maven') {
          steps {
            sh 'mvn --version'
          }
        }
      }
    }
    stage('build') {
      parallel {
        stage('bin') {
          steps {
            sh 'kubectl --version'
          }
        }
        stage('image') {
          steps {
            sh 'sudo docker --version'
          }
        }
      }
    }
    stage('deploy') {
      steps {
        echo 'success'
      }
    }
  }
}