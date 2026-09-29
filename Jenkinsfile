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
    stage('Create Artifact'){
      steps{
        sh 'echo "Jenkins Lab Artifact" > build-artifact.txt'
        archiveArtifacts artifacts: 'build-artifact.txt', fingerprint: true
  }
    }
  }
  post {
    success {
      echo 'Pipeline completed successfully!'
    }
  }
}
