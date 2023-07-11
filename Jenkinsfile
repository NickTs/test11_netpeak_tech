pipeline {

    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh "docker compose build"
            }
        }
        stage('Run') {
            steps {
                echo 'Runing...'
                sh "docker compose -f docker-compose.yml up -d"
            }
        }
    }
}
