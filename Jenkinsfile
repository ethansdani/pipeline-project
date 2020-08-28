pipeline {
	agent any
	stages {
		stage ('Fluffy Build') {
			steps {
				sh 'echo Placeholder > test.war'
				sh 'echo Edited Placeholder'
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
			}
		}
	}
}
