pipeline {
  agent {
    docker {
      image 'dombaink/phpngxver1'
    }

  }
   stages {
        stage('Test') {
            steps {
                sh 'docker --version'
            }
        }
    }
}
