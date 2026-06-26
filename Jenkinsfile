pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Deploy') {
            steps {
                sh 'cp index.html /var/www/html/index.html'
            }
        }
    }
}
