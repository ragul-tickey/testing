pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/ragul-tickey/testing.git'
            }
        }

        stage('Build') {
            steps {
                sh 'npm install' // Or any other build commands
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp -r * /var/www/html' // Copy your files to the web root
            }
        }
    }
}
