pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning repository...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'No build needed for static site. Just checking files...'
                sh 'ls -al'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying static site...'
                // For example, if you're copying to a directory (like /var/www/html)
                // You can replace this with AWS S3, FTP, rsync, etc.
                sh '''
                mkdir -p /tmp/static-site
                cp -r * /tmp/static-site/
                echo "Files copied to /tmp/static-site (or your target deploy directory)"
                '''
            }
        }
    }
}
