pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'invalid_command_here'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './hello_exec'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed!'
        }
    }
} 
