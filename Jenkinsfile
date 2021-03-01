pipeline {
  agent {
    docker {
      image 'node:lts-alpine3.12'
      args 'npm install'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'npm run build'
      }
    }

  }
  environment {
    PORT = '4000'
  }
}