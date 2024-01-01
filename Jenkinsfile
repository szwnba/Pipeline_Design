pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'hello world'
      }
    }
    triggers {
        cron('H/1 * * * *')
    }
    stage('test') {
      steps {
        echo 'test'
      }
    }

    stage('deploy') {
      steps {
        echo 'test deploy'
      }
    }

  }
}
