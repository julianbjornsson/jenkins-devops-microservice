pipeline {
	agent any
	stages {
		stage ('Build') {
			steps {
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