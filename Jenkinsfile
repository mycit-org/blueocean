pipeline {
  agent any
  stages {
    stage('mystage') {
      steps {
        echo 'hi'
      }
    }

    stage('yo') {
      parallel {
        stage('yo') {
          steps {
            echo 'yo'
          }
        }

        stage('parallel 2') {
          steps {
            echo 'parallel 2'
          }
        }

        stage('joe') {
          steps {
            echo 'Hey Ted'
          }
        }

      }
    }

  }
  environment {
    hello = 'world'
  }
}