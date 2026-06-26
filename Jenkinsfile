pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Test') {
            steps {
                sh 'test -f index.html && echo "index.html exists - PASS" || exit 1'
            }
        }
        stage('Deploy') {
            steps {
                sh 'cp index.html /var/www/html/index.html'
                sh 'echo "Deployed successfully!"'
            }
        }
    }
}
