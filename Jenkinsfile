pipeline {
    agent none
    stages {
        stage('python test') {
			agent {
				docker {
					image 'python:2-alpine'
				}
			}
			
            steps {
                sh 'python --version'
				echo 'python test case '
            }
        }
		
		stage('Java test') {
			agent {
				docker {
					image 'node:6.3'
				
				}
			}
			
			steps {
				sh 'npm --version'
				echo'Java test case'
			}
		}
		
		stage('Ruby test') {
			agent {
				docker {
					image 'ruby'
				}
			}
			
			steps {
                sh 'ruby --version'
				echo 'ruby test case.'
            }
		}
		
    }
}

