pipeline {
  agent any
  stages {
    stage('npm install') {
      steps {
        nodejs('nodejs') {
          sh 'npm install'
          sh 'cordova platform add android'
        }

      }
    }

    stage('cordova build android') {
      steps {
        nodejs('nodejs') {
          sh 'cordova build android --debug'
        }

      }
    }

  }
}