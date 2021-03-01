pipeline {
  agent any
  stages {
    stage('stage-1') {
      steps {
        sh 'git clone git@github.com:dextercdalogdog/backend-core.git'
      }
    }

  }
  environment {
    PORT = '3000'
  }
}