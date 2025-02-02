pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        echo 'hi how are your'
      }
    }

    stage('prod') {
      parallel {
        stage('prod') {
          steps {
            sh 'date'
          }
        }

        stage('cal') {
          steps {
            sh 'cal'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'final'
      }
    }

  }
}