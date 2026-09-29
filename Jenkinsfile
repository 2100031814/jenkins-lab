pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building application...'
      }
    }
    stage('Test'){
      steps {
        echo 'Running tests...'
      }
    }
    stage('Hello World'){
      steps{
        echo 'Hello World from Jenkins Pipeline!'
      }
    }
  }
  post {
    success {
      echo 'Pipeline completed successfully!'
    }
  }
}
