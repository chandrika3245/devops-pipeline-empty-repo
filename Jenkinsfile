pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'develop the ccode'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test the code'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy the code'
          }
        }

      }
    }

  }
}