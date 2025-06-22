stage('Deploy') {
    steps {
        echo 'Deploying static site...'
        sh '''
            mkdir -p /tmp/static-site
            cp index.html styles.css /tmp/static-site/
        '''
    }
}
