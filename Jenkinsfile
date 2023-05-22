pipeline {
	agent any
	tools {
		dockerTool 'Docker'
	}
	stages {
		stage("verifying tooling") {
			steps {
				sh '''
					service docker start
					docker version
					docker info
					docker compose version
					curl --version
					jq --version
				'''
			}
		}
	}
}