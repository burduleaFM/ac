pipeline {
  agent none
  stages {
    stage('image_build') {
      steps {
        sh 'docker-compose build'
        sh 'docker login -u alex199 -p trainer21!'
      }
    }

    stage('image_push') {
      steps {
        sh 'docker-compose push alex199/test_flask_app'
      }
    }

  }
}