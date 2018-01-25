pipeline {
    agent { docker 'node:6.3' }
    
    environment {
        DB_NAME      = 'DB_'
        DB_USER      = 'User'
    }

    stages {
        stage('build') {
            steps {
                sh 'printenv'
            }
        }
    }
}
