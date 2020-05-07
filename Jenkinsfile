pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        node(label: 'nodejs') {
          sh 'npm install'
        }

      }
    }

  }
}