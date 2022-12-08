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
        sh 'sudo npm cache clean --force'
        sh 'npm ci'
      }
    }
    stage('run') {
      steps {
        sh 'echo "run"'
      }
    }
  }
}
