pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build done'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test'
          }
        }

        stage('test1') {
          steps {
            echo 'teste1'
          }
        }

        stage('test2') {
          steps {
            echo 'test2'
          }
        }

        stage('test3') {
          steps {
            echo 'test3'
          }
        }

      }
    }

    stage('depley') {
      steps {
        echo 'deploy'
      }
    }

  }
}