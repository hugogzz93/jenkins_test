pipeline {
    agent { docker 'pinelo93/jenkins_test:latest' }
    stages {
        stage('build') {
            steps {
                sh 'bundle exec rake'
            }
        }
    }
}
