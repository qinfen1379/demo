#!/usr/bin/env groovy

pipeline {
    agent any
    stages {
        stage('Example stage 1') {
            environment {
                BITBUCKET_COMMON_CREDS = credentials('jenkins-bitbucket-common-creds')
            }
            steps {
                echo 'val is ${BITBUCKET_COMMON_CREDS}'
            }
        }
        stage('Example stage 2') {
            steps {
                echo 'securt username and passwd is right'
            }
        }
    }
}
