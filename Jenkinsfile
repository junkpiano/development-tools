pipeline {
    agent {
        docker { image 'ruby:latest' }
    }
    stages {
        stage('Test') {
            steps {
                sh'''
                bundle
                bundle exec danger
                '''
            }
        }
    }
}