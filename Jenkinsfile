pipeline {
  agent {
    docker {
      image 'dombaink/phpngxver1'
      args '-p 8082:8080'
    }

  }
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh '''ls -al
docker ps'''
          }
        }
        stage('pull') {
          steps {
            sh 'git clone https://github.com/dombaink/laravel.git'
          }
        }
      }
    }
  }
}