pipeline {
  environment {
    registry = "aravindhanravi003/docker-test"
    registryCredential = 'dockerHub'
    dockerImage = ''
  }
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/Aravindhan-003/dockerpipeline.git'
      }
    }
   stage('Building image') {
      steps{
        script {
          docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
  }
}
