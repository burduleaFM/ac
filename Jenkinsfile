pipeline {
  agent none
  stages {
    stage('image_build') {
      steps {
        sh 'docker-compose build'
      }
    }

    stage('image_push') {
      steps {
        sh 'docker-compose push alex199/test_flask_app'
      }
    }

  }
}