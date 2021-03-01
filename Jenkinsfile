pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        sh 'docker build . -t dextercdalogdog/backend-core:latest'
      }
    }

    stage('RUN') {
      steps {
        sh 'docker run -d -p 3000:3000 dextercdalogdog/backend-core:latest'
      }
    }

  }
  environment {
    PORT = '4000'
  }
}