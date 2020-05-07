pipeline {
  agent any
  stages {
    stage('tool npm') {
      steps {
        tool 'nodejs'
      }
    }

    stage('npm install') {
      steps {
        sh 'npm install'
      }
    }

  }
}