pipeline {
	agent any
	tools {
		maven 'maven'
		// jdk 'java-8'
	}
	stages {
		stage('git-code-checkout'){
			steps {
				git "https://github.com/himabindu7702/devops-batch.git"
			}
		}
		stage('maven-build'){
			steps {
				sh 'clean install package -DskipTests'
				}
			}
		}
}
