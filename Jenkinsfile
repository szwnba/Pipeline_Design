pipeline {
  agent {
    docker {
      image 'python:3.9-alpine'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'pip -V'
      }
    }

    stage('Schedule') {
      steps {
        echo 'H/4 * * * *'
      }
    }

    stage('Get news') {
      parallel {
        stage('Get news') {
          steps {
            echo 'get news'
          }
        }

        stage('Get news2') {
          steps {
            echo 'Get news'
          }
        }

        stage('Get news3') {
          steps {
            echo 'Get news'
          }
        }

      }
    }

    stage('Ai transfer') {
      steps {
        echo 'test deploy'
      }
    }

    stage('Email') {
      steps {
        echo 'Email to me when failed'
      }
    }

  }
}