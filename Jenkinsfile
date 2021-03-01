pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        git(credentialsId: 'jenkins-to-repo', url: 'https://github.com/dextercdalogdog/backend-core', branch: 'main')
      }
    }

  }
  environment {
    PORT = '3000'
  }
}