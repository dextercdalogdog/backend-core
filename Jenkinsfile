pipeline {

    agent any

    stages {

        stage ('Initialization') {
            steps {
                sh 'echo "Starting the build"'
            }
        }

        stage ('Build') {
            steps {
                sh 'npm install'
            }
        }
      
        stage ('NPM Audit Analysis') {
            steps {
                sh '/{PATH TO SCRIPT}/npm-audit.sh'
            }
        }

        stage ('NodeJsScan Analysis') {
            steps {
                sh 'nodejsscan --directory `pwd` --output /{JENKINS HOME DIRECTORY}/reports/nodejsscan-report'
            }
        }
    }

}
