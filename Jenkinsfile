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
        input(message: 'TEST-ok', ok: 'test')
        build 'terawebdev'
      }
    }
  }
}