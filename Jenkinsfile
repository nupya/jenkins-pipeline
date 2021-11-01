pipeline {
	agent any
	triggers { pollSCM 'H/1 * * * *' }
	stages {
		stage('One') {
			steps {
				echo 'Hi, this is Nupoor welcome you here'
			}
		}
		
		stage('Two') {
			steps {
				input('Do you want to proceed further?')
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
        
        stage('Check') {
            steps {
                bat './gradlew check'
            }
        }      
		
		stage('Five') {
			steps {
				echo 'Finished'
			}
		}		
	}
}
