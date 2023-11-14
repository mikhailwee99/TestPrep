pipeline {
	    agent any

		stages {
			stage('Start Local HTTP Server') {
				steps {
					script {
						// Start a simple HTTP server on port 8080
						sh 'python -m http.server 8080 &'
						
						// Sleep for a while to ensure the server has started
						sleep time: 10, unit: 'SECONDS'
					}
				}
			}
		}
	}
