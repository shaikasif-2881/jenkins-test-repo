
pipeline {
    agent {
        docker {
            image 'python:3.10'
        }
    }

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Run Python') {
            steps {
                sh '''
                python --version
                python app.py
                '''
            }
        }
    }
}
