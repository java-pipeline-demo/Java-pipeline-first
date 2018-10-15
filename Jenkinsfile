pipeline {
  agent {
    label 'jdk8'
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