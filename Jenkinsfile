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
ls -al'''
          }
        }
        stage('pull') {
          steps {
            sh 'git clone https://github.com/dombaink/laravel.git ./test'
          }
        }
      }
    }
    stage('build code') {
      parallel {
        stage('build docker') {
          steps {
            sh 'echo "build code"'
          }
        }
        stage('deploy code') {
          steps {
            sh 'echo "test"'
          }
        }
      }
    }
  }
}