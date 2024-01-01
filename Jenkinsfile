pipeline {
  agent any
   triggers {
       cron('H/1 * * * *')
  }
  
  stages {
    stage('build') {
      steps {
        echo 'hello world'
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
}
