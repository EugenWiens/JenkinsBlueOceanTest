pipeline {
  agent any
  stages {
    stage('print') {
      parallel {
        stage('print') {
          steps {
            echo 'hellow'
          }
        }
        stage('') {
          steps {
            input(message: 'Hallo', id: 'TEST', ok: 'OKy', submitter: 'SubmitterText', submitterParameter: 'SubmitterParameterText')
          }
        }
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