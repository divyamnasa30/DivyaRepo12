pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'i want to plan my app'
      }
    }

    stage('code') {
      steps {
        echo 'dev team performs dev'
      }
    }

    stage('build') {
      steps {
        echo 'build the app'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test it'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy files'
          }
        }

        stage('Release') {
          steps {
            echo 'move'
          }
        }

        stage('operate') {
          steps {
            echo 'test app'
          }
        }

      }
    }

  }
}