pipeline {
	agent any
	stages {
		stage("verifying tooling") {
			steps {
				sh '''
					sudo docker version
					sudo docker info
					sudo docker compose version
					curl --version
					jq --version
				'''
			}
		}
	}
}