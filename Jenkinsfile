pipeline {
    agent { docker 'pinelo93/jenkins_test:latest' }
    stages {
        stage('setup') {
            steps {
                sh 'gem install rubocop'
            }
        }
        stage('test') {
            steps {
                sh 'bundle exec rake'
            }
        }
        stage('rubocop') {
          steps {
                sh 'bundle exec rubocop'
            }
        }
    }
}
