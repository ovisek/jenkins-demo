pipeline {
	agent any
	stages {
		stage ('build') {
            		steps {
                		echo "building phase"
				withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: 'sf-sys-jenkins-account credential store', usernameVariable: 'JENKINS_USERNAME', passwordVariable: 'JENKINS_PASSWORD']])
				{
					echo "${JENKINS_USERNAME}"
					echo "${JENKINS_PASSWORD}"
				}
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
		always {
			echo "All phases are complete now"
		}
	}
}
