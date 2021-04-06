
pipeline{
	agent {  docker { image 'python'} }
	stages {
		stage('Build'){
			steps {
				sh 'python --version'
				echo "Build"
			}
		}
		stage('Test'){
			steps {
				echo "Test"
			}
		}
		stage('Integration test'){
			steps {
				echo "Integration test"
			}
		}
	}
	post {
		always {
			echo "I always run"
		}
		success {
			echo "I run on success"
		}
		failure {
			echo "I run on failure"
		}
	}
}
