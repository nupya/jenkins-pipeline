pipeline {
	agent any
	triggers { pollSCM 'H/1 * * * *' }
	stages {
		stage('One') {
			steps {
				echo 'Hi, this is Nupoor welcome you here'
			}
		}
		
		stage('Build') {
            steps {
                bat './gradlew build'
            }
        }
        
        stage('Test') {
            steps {
                bat './gradlew test'
            }
        }
        
       
		
		stage('Five') {
			steps {
				echo 'Finished'
			}
		}		
	}
}
