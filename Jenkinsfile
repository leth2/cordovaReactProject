pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh 'npm install'
        withNPM()
        node(label: 'nodejs') {
          sh 'npm install'
        }

      }
    }

  }
}