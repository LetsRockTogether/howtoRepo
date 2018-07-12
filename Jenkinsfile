pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('SayHello') {
      steps {
        echo 'Hello World'
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Anshu'
  }
}