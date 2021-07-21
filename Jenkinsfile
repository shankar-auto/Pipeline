pipeline {
	agent any  
	stages {
		stage('Stage1') {
			steps {
				echo "Stage 1 is running ----"
				sh 'sleep 5'
				sh 'exit 1'
			}	
		}
		stage('Stage2') {			
			steps {
				echo "Stage 2 is Running ----"
				sh 'sleep 5'
			}
		}
	}
}
				
	



