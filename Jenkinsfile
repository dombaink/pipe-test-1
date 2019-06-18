pipeline {
  agent {
    docker {
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