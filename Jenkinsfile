pipeline {
	agent any  
	parameters {
		//string(name: 'TARGET_ENV', description: 'Target Environment to display')
		choice(name: 'TARGET_ENV', choices: {'test', 'prod'}, description: 'Target Environment to display'
	}
	environment {
		DEPLOY_TO = "${TARGET_ENV}"
	}
	stages {
		stage('DEPLOY_TEST') {
			when {
				environment name: 'DEPLOY_TO', value: 'test'
			}
			steps {				
				echo "DEPLOY To TEST Environment ----"
				sh 'sleep 5'
				
			}	
		}
		stage('DEPLOY_PROD') {
			when {
				environment name: 'DEPLOY_TO', value: 'prod'
			}
			steps {
				echo "DEPLOY TO PROD ENVIRONMENT----"
				sh 'sleep 5'
			}
		}
	}
}
