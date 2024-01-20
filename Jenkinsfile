pipeline {
  agent any
  stages {
    stage('Development') {
      steps {
        echo 'This is Dev Stage'
      }
    }

    stage('Testing') {
      parallel {
        stage('Testing') {
          steps {
            echo 'This is Testing stage.'
          }
        }

        stage('UAT') {
          steps {
            echo 'UAT started'
          }
        }

        stage('Integration') {
          steps {
            echo 'Integration started.'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'This is Build stage.'
      }
    }

    stage('Deploy') {
      steps {
        echo 'This is Deploy stage.'
      }
    }

  }
}