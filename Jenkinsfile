pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test ') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'testing Firefox\'; exit 1'
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrome\''
          }
        }

        stage('Test edge') {
          steps {
            sh 'echo \'test edge\''
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}
