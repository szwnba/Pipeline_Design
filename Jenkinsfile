pipeline {
  agent any
  stages {
    stage('Schedule') {
      steps {
        echo 'plan'
      }
    }
    
    stage('Get news') {
      steps {
        echo 'get news'
      }
    }

    stage('Ai transfer') {
      steps {
        echo 'test deploy'
      }
    }

    stage('Email') {
      steps {
        echo 'Email to me'
      }
    }

  }
  triggers {
    cron('H/4 * * * *')
  }
}
