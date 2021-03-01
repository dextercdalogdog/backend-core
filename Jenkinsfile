pipeline {
  agent any
  stages {
    stage('stage-1') {
      steps {
        git(url: 'https://github.com/dextercdalogdog/backend-core', branch: 'main')
      }
    }

  }
  environment {
    PORT = '3000'
  }
}