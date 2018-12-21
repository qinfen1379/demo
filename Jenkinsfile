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
            junit '**/target/*.xml'
        }
        failure {
            mail to} qinfen_python@163.com, subject: 'The Pipeline failed :('
        }
    }
}
