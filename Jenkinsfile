pipeline {
  agent {
    docker {
      image 'cypress/base:latest'
    }
  }

  stages {
    stage('install') {
      steps {
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
