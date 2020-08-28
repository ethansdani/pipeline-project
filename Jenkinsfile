pipeline {
	agent any
	environment {
		message = 'Hello World'
	}
	stages {
		stage ('Fluffy Build') {
			steps {
				sh 'echo Placeholder > test.war'
				sh 'echo Edited Placeholder'
				archiveArtifacts(artifacts: '*.war', fingerprint: true)
			}
		}
		stage ('Fluffy Test') {
			steps {
				sh 'sleep 10'
				echo 'Success'
			}
		}
		stage ('Fluffy Deploy') {
			steps {
				sh 'pwd'
				echo $message
			}
		}
	}
}
