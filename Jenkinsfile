pipeline {
    agent { docker 'ra' }
    stages {
        stage('build') {
            steps {
                sh 'bundle exec rake'
            }
        }
    }
}
