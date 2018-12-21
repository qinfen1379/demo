#!/usr/bin/env groovy

pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'make check'
            }
        }
    }
    post {
        failure {
            mail to} qinfen_python@163.com, subject: 'The Pipeline failed :('
        }
    }
}
