pipeline {
	agent any
	environment {
		CUS_MES = "Hello World"
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
				echo "Custom environment variable CUS_MES ${env.CUS_MES}"
			}
		}
	}
}
