pipeline {
  agent {
    docker {
      image 'dombaink/phpngxver1'
      args '-p 8082:8080'
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