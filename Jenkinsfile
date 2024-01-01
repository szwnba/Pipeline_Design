pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'hello world'
          }
        }

        stage('build2') {
          steps {
            echo 'test bulid2'
          }
        }

      }
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
  triggers {
    cron('H/4 * * * *')
  }
}
