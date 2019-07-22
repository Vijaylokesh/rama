pipeline {
   environment {
    registry = "vijaylokesh/rama"
    registryCredential = 'docker-hub'
    dockerImage = ''
    }
  agent {
    label 'docker_slave1'
  } 
  stages {
    stage('Cloning Git') {
      steps {
        git 'https://github.com/Vijaylokesh/rama.git'
      }
    }
    stage('Building image') {
      steps{
        script {
          dockerImage = docker.build registry + ":latest"
        }
      }
    }

