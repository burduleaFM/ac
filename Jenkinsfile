pipeline {
  agent any
  stages {
    stage('image_build') {
      steps {
        sh 'docker-compose build'
        sh 'docker login -u alex199 -p trainer21!'
      }
    }

    stage('image_push') {
      steps {
        sh 'docker-compose push '
      }
    }

  }
}