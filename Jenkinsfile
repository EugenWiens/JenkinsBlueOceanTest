pipeline {
  agent any
  stages {
    stage('print') {
      steps {
        echo 'hellow'
      }
    }
    stage('echo1') {
      parallel {
        stage('echo1') {
          steps {
            sh 'echo "shell 1"'
          }
        }
        stage('echo2') {
          steps {
            sh 'echo "echo2"'
          }
        }
      }
    }
  }
}