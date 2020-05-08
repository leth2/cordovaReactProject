pipeline {
  agent any
  stages {
    stage('cordova build') {
      steps {
        nodejs('nodejs') {
          sh 'npm install'
          sh 'npm install -g cordova'
          sh 'cordova platform add android'
          withGradle() {
            sh 'cordova build android --debug'
          }

        }

      }
    }

    stage('get artifact') {
      steps {
        archiveArtifacts(artifacts: '*/build/**/*.apk', onlyIfSuccessful: true)
      }
    }

  }
}