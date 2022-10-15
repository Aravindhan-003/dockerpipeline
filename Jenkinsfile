pipeline {
  environment {
    registry = "aravindhanravi003/docker_automation"
    registryCredential = 'docker'
    dockerImage = ''
  }
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/Aravindhan-003/dockerpipeline.git'
      }
    }
  }
}
