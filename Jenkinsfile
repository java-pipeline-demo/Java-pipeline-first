pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Initial') {
      steps {
        echo "Hello ${params.Name}!"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
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
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}