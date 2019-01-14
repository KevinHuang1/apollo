pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sleep 5
      }
    }
    stage('echo') {
      parallel {
        stage('echo') {
          steps {
            echo 'hello'
          }
        }
        stage('echo1') {
          steps {
            pwd()
          }
        }
      }
    }
  }
}
