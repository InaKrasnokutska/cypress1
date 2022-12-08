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
        sh 'npm i'
      }
    }
    stage('run') {
      steps {
        sh 'echo run'
      }
    }
  }
}
