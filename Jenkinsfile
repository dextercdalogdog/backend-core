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

    stage('') {
      steps {
        sh 'docker build . -t dextercdalogdog/backend-core:latest'
      }
    }

  }
  environment {
    PORT = '4000'
  }
}