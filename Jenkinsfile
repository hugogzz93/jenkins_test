pipeline {
    agent { docker 'pinelo93/jenkins_test:latest' }
    stages {
        stage('test') {
            steps {
                sh 'bundle exec rake'
                sh 'bundle exec rubocop'
            }
        }
    }
}
