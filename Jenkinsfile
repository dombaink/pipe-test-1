pipeline {
  agent {
    docker {
      image 'dombaink/phpngxver1'
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