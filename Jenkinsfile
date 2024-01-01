pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'hello world'
      }
    }

    stage('deploy') {
      steps {
        echo 'test deploy'
      }
    }

  }
  triggers {
    cron('H/4 * * * *')
  }
}