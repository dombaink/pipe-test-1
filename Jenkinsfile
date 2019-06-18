pipeline {
  agent {
    dockerfile {
      filename 'Dokerfile'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'docker build -t dombaink/phpngx:v1 .'
      }
    }
  }
}