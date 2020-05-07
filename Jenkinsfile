pipeline {
  agent any
  stages {
    stage('npm install') {
      steps {
        withNPM() {
          sh 'npm install'
        }

      }
    }

    stage('cordova Build') {
      steps {
        withNPM() {
          sh 'cordova build'
        }

      }
    }

  }
}