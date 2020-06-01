pipeline {
	agent {
        docker { image 'node:7-alpine' }
    }
	stages {
		stage ('Build') {
			steps {
				sh 'mvn --version'
				echo "Build"
			}
		}
		stage ('Test') {
			steps {
				echo "Test"
			}
		}
		stage ('Integration Test') {
			steps {
				echo "Integration test"
			}
		}
	} 
    
    post {
        always {
            echo 'SIEMPRE'
        }
        success {
            echo 'SUCCESSFULLY RUN'
        }
        failure {
            echo 'FAILURE'
        }
    }
}