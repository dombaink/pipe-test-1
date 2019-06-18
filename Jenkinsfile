pipeline {
  agent {
    docker {
      args 'docker ps '
      image 'dombaink/phpngxver1'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'docker ps -a'
      }
    }
  }
}