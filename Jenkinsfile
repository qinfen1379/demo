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
        always {
            mail to:qinfen_python@163.com, subject: 'the pipeline is ok :('
        }
        failure {
            mail to:qinfen_python@163.com, subject: 'the pipeline is failed :('
        }
    }
}
