pipeline {
    agent any

    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/mohamedmohsen20/netty-example.git'
            }
        }
        stage('maven Build') {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
