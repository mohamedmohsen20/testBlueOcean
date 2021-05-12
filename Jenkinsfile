pipeline {
    agent any

    stages {
        stage('git checkout') {
            steps {
                echo "start git checkout stage"
                git 'https://github.com/mohamedmohsen20/netty-example.git'
            }
        }
        stage('maven Build') {
            steps {
                echo "start maven build stage"
                sh "mvn clean package"
            }
          
        }
        stage('maven test') {
            steps {
                echo 'start maven test stage'
                sh 'mvn package'
            }
                     
        }

        stage('maven package') {
            steps {
                echo 'start maven package stage'
                sh 'mvn package'
            }
    }
}
