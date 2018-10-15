pipeline {
  agent {
    label 'jdk10'
  }
  stages {
    stage('Initial') {
      steps {
        echo 'Hello World'
      }
    }
    stage('Script') {
      steps {
        sh 'java -version'
      }
    }
  }
}