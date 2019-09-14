pipeline {
	agent Jenkins-Slave-1
	stages {
		stage('---clean---'){
			steps {
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				sh "mvn test"
			}
		}
		stage('---package---') {
			steps {
				sh "mvn package"
			}
		}
	}
}
