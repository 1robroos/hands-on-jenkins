pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo \'testing Firefox\''
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo \'Testing Chrome\''
          }
        }

        stage('Test edge') {
          steps {
            sh 'echo \'test edge in this branch\''
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
