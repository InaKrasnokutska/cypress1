pipeline {
  agent {
    docker {
      image 'cypress/base:latest'
    }
  }

  stages {
    stage('install') {
      steps {
        sh 'ls'
      }
    }
    stage('run') {
      steps {
        sh 'docker build -t cypress .'
      }
    }
  }
}
