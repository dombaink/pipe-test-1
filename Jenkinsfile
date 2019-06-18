pipeline {
  agent {
    docker {
      image 'dombaink/nginx-php7'
      args 'docker ps '
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