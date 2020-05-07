pipeline {
  agent any
  stages {
    stage('tool npm') {
      steps {
        nodejs('nodejs') {
          sh 'npm install'
        }

      }
    }

    stage('') {
      steps {
        nodejs('nodes') {
          sh 'cordova build android --debug'
        }

      }
    }

  }
}