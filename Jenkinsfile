pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/gradekam/projects.git', branch: 'master')
      }
    }

    stage('Maven build') {
      steps {
        sh '''echo %cd%
cd "C:\\Users\\Anna\\Documents\\selenium-training-master"
echo %cd%
mvn test'''
      }
    }

  }
  environment {
    BRANCH = 'master'
  }
}