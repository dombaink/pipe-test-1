pipeline {
  agent {
    dockerfile {
      filename 'Dokerfile'
    }

  }
  stages {
    stage('build') {
      steps {
        sh 'docker build -t dumbaink/phpngx .'
      }
    }
  }
}