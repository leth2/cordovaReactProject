pipeline {
  agent any
  stages {
    stage('npm install') {
      steps {
        nodejs('nodejs') {
          sh 'npm install'
        }

      }
    }

    stage('error') {
      steps {
        nodejs('nodejs') {
          sh 'cordova build android --debug'
        }

      }
    }

  }
}