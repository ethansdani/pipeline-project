pipeline {
	agent any
	environment {
		CUS_MES = "Hello World"
	}
	stages {
		parallel {
			stage ('Fluffy Build1') {
				steps {
					echo "This is build1"
				}
			}
			stage ('Fluffy Build2') {
				steps {
					echo "This is build2"
				}
			}
		}
		stage ('Fluffy Test') {
			steps {
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
