pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'echo " build is run"'
      }
    }
    stage('cloud') {
      steps {
        sh 'echo " hai"'
      }
    }
  }
}