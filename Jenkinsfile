pipeline {
  agent {
    docker {
      image 'cypress/base:latest'
    }
  }

  stages {
    stage('install') {
      steps {
        sh 'rm -rf package-lock.json'
        sh 'npm ci'
      }
    }
    stage('run') {
      steps {
        sh 'echo run'
      }
    }
  }
}
