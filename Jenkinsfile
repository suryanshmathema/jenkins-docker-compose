pipeline {
	agent any
	tools {
		dockerTool 'Docker'
	}
	stages {
		stage("verifying tooling") {
			steps {
				sh '''
					dockerd
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