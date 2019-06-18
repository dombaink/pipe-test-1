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
mkdir test
ls -al '''
          }
        }
        stage('pull') {
          steps {
            sh 'git cloneÂ https://github.com/dombaink/laravel.git'
          }
        }
      }
    }
  }
}