pipeline {
    stages {
	    agent {
				docker {
					image 'ubuntu'
				}
        }
        stage('build') {
 
            steps{
                echo "building phase"
                sh "uname -a"
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