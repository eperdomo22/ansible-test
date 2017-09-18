pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'hello world'
      }
    }
    stage('docker') {
      steps {
        library 'DOCKERLIB'
      }
    }
    stage('test3') {
      steps {
        retry(count: 2)
        input(message: 'TEST-ok', ok: 'test')
      }
    }
  }
}