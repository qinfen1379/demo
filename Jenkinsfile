#!/usr/bin/env groovy

pipeline {
    agent any
	def username = "qinfen"
    stages {
        stage('Build') {
            steps {
				echo "my name is ${username}"
				echo "Running ${env.BUILD_ID}"
            }
        }
    }
}
