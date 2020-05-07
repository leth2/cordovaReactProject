pipeline {
  agent any
  stages {
    stage('npm install') {
      steps {
        sh 'npm install'
      }
    }

    stage('cordova Build') {
      steps {
        sh 'cordova build'
      }
    }

  }
}