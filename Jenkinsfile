pipeline {
  agent {
    docker {
      image 'node:10-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'yarn install'
        echo 'hello'
        sh 'echo $PATH'
        echo 'good'
      }
    }

  }
  environment {
    CI = 'true'
  }
}