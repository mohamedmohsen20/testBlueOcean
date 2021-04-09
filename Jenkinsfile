pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build completed'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo "test"'
          }
        }

        stage('test1') {
          steps {
            echo 'running test 1'
          }
        }

        stage('TEST2') {
          steps {
            echo 'tets 2'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy has finshed'
      }
    }

  }
}