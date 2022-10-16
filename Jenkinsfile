pipeline {
  environment {
    dockerImage = ''
    dockerImg = ''
    dockerIm = ''
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
          dockerImage = 'docker build -t aravindhanravi003/docker-test .'
        }
       }
      }
       stage('Deploy Image') {
      steps{
         script {
             dockerImg= 'docker tag docker-test aravindhanravi003/docker-test'
             dockerIm= 'docker push aravindhanravi003/docker-test'
         }
       }
      }
    }
  }


