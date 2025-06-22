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
                echo 'No build needed for static site.'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Deploying static site..."
                mkdir -p /tmp/static-site
                cp index.html /tmp/static-site/
                cp styles.css /tmp/static-site/
                echo "Files copied to /tmp/static-site"
                '''
            }
        }
    }
}
