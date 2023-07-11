pipeline {

    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh "docker compose build"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh "docker compose up -d"
            }
        }
    }
}
