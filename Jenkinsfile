#!/usr/bin/env groovy
pipeline {
    agent any 
        stages {
            stage('Build') {
                steps {
                    sh 'make check || true'
                    junit '**/target/*.xml'
                    echo 'hello jenkins test'
                }
            }
        }
}
