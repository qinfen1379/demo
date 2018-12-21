#!/usr/bin/env groovy

pipeline {
    agent any
    stages {
        stage('Build') {
			def username = "qinfen"
            steps {
				echo "my name is ${username}"
				echo "Running ${env.BUILD_ID}"
            }
        }
    }
}
