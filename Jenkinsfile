pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('dev') {
      steps {
        echo "Hello ${params.Name}!"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Kumar'
    TEST_USER = credentials('test-user')
  }
}