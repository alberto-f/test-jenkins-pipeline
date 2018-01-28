pipeline {
    agent { docker 'node:6.3' }
    
    stages {
        stage('build') {
            steps {
                sh 'echo "step 1"'
		sh 'echo "step 2"'
            }
        }

	stage('test') {
	    steps {
		sh 'echo "Test starting"'
		sh 'echo "Test finished"'
	    }
	}

	stage('deploy'){
	    steps {
		sh 'echo "Deplying"'
		sh 'echo "Deplying finished"'
	    }
	}
    }
    post {
        always {
          echo 'Done.'
        }
        
        changed {
          echo 'Pipeline changes status.'
        }
    }
}
