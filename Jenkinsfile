pipeline {
  agent {
    docker {
      image 'cypress/base:latest'
    }
  }

  stages {
    stage('install') {
      steps {
        sh 'sudo chown -R 994:991 "/.npm"'
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
