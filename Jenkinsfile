#!/usr/bin/env groovy
pipeline {
    agent any 
        stages {
            stage('Depoly') {
            when {
                expression {
                    currentBuild.result == null || currentBuild.result == 'SUCCESS'
                    }
                  }
            steps {
                sh 'make publish'

                }
            }
        }
}
