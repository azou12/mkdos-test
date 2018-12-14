pipeline {
  agent {
    docker {
      args '-v $WORKSPACE:/docs --entrypoint bash'
      image 'python 2.7'
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