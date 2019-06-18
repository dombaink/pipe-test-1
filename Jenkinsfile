pipeline {
  agent {
    docker {
      image 'dombaink/phpngxver1'
      args '-p 8081:8080'
    }

  }
  stages {
    stage('') {
      steps {
        sh 'docker ps -a'
      }
    }
  }
}