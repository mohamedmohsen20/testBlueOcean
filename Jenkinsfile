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
    }
}
