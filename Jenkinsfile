pipeline {
  agent any
  stages {
    stage('npm install') {
      steps {
        node(label: 'nodejs') {
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