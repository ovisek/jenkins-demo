pipeline {
	agent any
    stages {
        stage('build') {
            steps{
                echo "building phase"
            }
        }
        stage('test') {
            
            steps{
                echo "testing phase"
            }
        }
        stage('deploy') {
            steps{
                echo "deploy phase"
            }
        }
    }
	post {
		success {
			
		}
		always {
			echo "All phases are complete now"
		}
	}
}