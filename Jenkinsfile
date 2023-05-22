pipeline {
	agent any
	tools {
		dockerTool 'Docker'
	}
	stages {
		stage("verifying tooling") {
			steps {
				sh '''
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