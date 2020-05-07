pipeline {
  agent any
  stages {
    stage('npm install') {
      steps {
        nodejs('nodejs') {
          sh 'npm install'
          sh 'cordova build android --release'
        }

      }
    }

  }
}