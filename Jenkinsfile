pipeline {
  agent any
  stages {
    stage('cordova build') {
      steps {
        nodejs('nodejs') {
          sh 'npm install'
          sh 'cordova build android --debug'
        }

      }
    }

  }
  environment {
    PATH = '/usr/local/bin:/usr/bin:/bin'
  }
}