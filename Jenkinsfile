pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'hello world'
      }
    }
    stage('build') {
      steps {
        pwd()
      }
    }
    stage('docker') {
      steps {
        library 'DOCKERLIB'
      }
    }
  }
}