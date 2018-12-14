pipeline {
  agent {
    docker {
      image 'squidfunk/mkdocs-material'
      args '-v $WORKSPACE:/docs'
    }

  }
  stages {
    stage('build') {
      steps {
        sh '''mkdos build

'''
      }
    }
  }
}