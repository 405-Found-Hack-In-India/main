pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/405-Found-Hack-In-India/main', branch: 'master')
      }
    }

    stage('logs') {
      parallel {
        stage('logs') {
          steps {
            sh 'ls -la'
          }
        }

        stage('') {
          steps {
            sh 'cd main && npm i && npm i run test:unit'
          }
        }

      }
    }

  }
}