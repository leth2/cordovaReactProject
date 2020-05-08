pipeline {
  agent any
  stages {
    stage('npm install') {
      parallel {
        stage('npm install') {
          steps {
            nodejs('nodejs') {
              sh 'npm install'
            }

          }
        }

        stage('cordova add android') {
          steps {
            nodejs('nodejs') {
              sh 'cordova platform add android'
            }

          }
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