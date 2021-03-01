pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        git(credentialsId: 'jenkins-to-repo', url: 'https://github.com/dextercdalogdog/backend-core', branch: 'main')
        sh 'docker build . -t dextercdalogdog/frontend-core:2021.03.01'
      }
    }

  }
  environment {
    PORT = '3000'
  }
}