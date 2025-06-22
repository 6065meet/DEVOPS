stage('Deploy') {
    steps {
        sh '''
        mkdir -p /tmp/static-site
        cp index.html /tmp/static-site/
        cp styles.css /tmp/static-site/
        echo "Files copied to /tmp/static-site/"
        '''
    }
}
