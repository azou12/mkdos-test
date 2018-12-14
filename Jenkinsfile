pipeline {
  agent {
    docker {
      image 'squidfunk/mkdocs-material'
      args '-v $WORKSPACE:/docs --entrypoint'
    }

  }
  stages {
    stage('build') {
      steps {
        sh '''mkdocs build

'''
      }
    }
  }
}