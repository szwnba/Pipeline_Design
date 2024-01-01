pipeline {
  agent {
        docker {
            image 'maven:3-alpine'
            args '-v /root/.m2:/root/.m2'
        }
    }
	
  stages {
		stage('Build') {
            steps {
                sh 'mvn -version'
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
