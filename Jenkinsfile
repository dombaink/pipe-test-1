pipeline {
  agent {
    docker {
      image 'dombaink/phpngxver1'
      args '-u 0:0 8081:8080'
    }

  }
  stages {
    stage('error') {
      steps {
        sh 'run -p 8081:8080'
      }
    }
  }
}