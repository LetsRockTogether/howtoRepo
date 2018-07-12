pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('SayHello') {
      steps {
        echo 'Hello World'
        echo "Hello ${MY_NAME}!"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        sh 'java -version'
      }
    }
  }
  environment {
    TEST_USER = credentials('test-user')
    MY_NAME = 'Anshu'
  }
}