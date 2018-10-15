pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Initial') {
      steps {
        echo "Hello ${MY_NAME}!"
      }
    }
    stage('Script') {
      steps {
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Anant'
  }
}