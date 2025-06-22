pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'No build needed for static site.'
                sh 'ls -al'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Copying files to /tmp/static-site'
                sh '''
                    mkdir -p /tmp/static-site
                    cp index.html styles.css /tmp/static-site/
                '''
            }
        }
    }
}
