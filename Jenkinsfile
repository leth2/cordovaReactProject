pipeline {
  agent any
  stages {
    stage('npm install') {
      steps {
        nodejs('nodes') {
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