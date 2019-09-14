pipeline {
	agent any
	stages {
		stage('---clean---'){
			steps {
				sh "mvn clean"
			}
		}
		stage('---test---') {
			steps {
				tool name: 'mvn3.3.3', type: 'maven'
				sh "mvn test"
			}
		}
		stage('---package---'){
			steps {
				tool name: 'mvn3.3.3', type: 'maven'
				sh "mvn package"
			}
		}
	}
}
