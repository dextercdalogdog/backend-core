pipeline {
  agent {
    docker {
      image 'node:lts-alpine3.12'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'npm install'
        sh 'npm run build'
      }
    }

  }
  environment {
    PORT = '4000'
  }
}