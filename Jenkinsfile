#!/usr/bin/env groovy

pipeline {

    agent {
        docker {
            image 'wordpress:5.1.1-fpm-alpine'
            args '-u root'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                #sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                #sh 'npm test'
            }
        }
    }
}
