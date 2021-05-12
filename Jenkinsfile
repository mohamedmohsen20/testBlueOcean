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
                sh "mvn clean "
            }
        }
        stage('maven test') {
            steps {
                echo "start maven test stage"
                sh "mvn test "
            }
        }
        stage('maven package') {
            steps {
                echo "start maven package stage"
                sh "mvn package "
            }
        }
        stage('build image') {
            steps {
                echo "start docker"
                sh "docker build -t ci-cd:${BUILD_NUMBER} . "
                
            }
        }
        
    }
}
