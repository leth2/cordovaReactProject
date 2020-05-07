pipeline {
  agent any
  stages {
    stage('npm install') {
      parallel {
        stage('npm install') {
          steps {
            sh 'npm install'
          }
        }

        stage('cordova build') {
          steps {
            sh 'cordova build'
          }
        }

      }
    }

  }
}