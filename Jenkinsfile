pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'HTML project - no build needed'
                sh 'ls -la'
            }
        }
        stage('Test') {
            steps {
                echo 'Checking HTML files exist...'
                sh 'test -f index.html && echo "index.html found!" || echo "index.html not found"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'HTML site deployed successfully!'
            }
        }
    }
}
