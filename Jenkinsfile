pipeline {
	agent any  
	stages {
		stage('BUILD') {
			steps {
				sh '''
					pwd
					sleep 5
					echo This is the fist stage: BUILD
				'''
			}	
		}
		
		stage('TEST') {
			parallel{
				stage('TEST1') {					
					steps {
						sh 'sleep 5'
						echo "Testing Parallel"
					}
				}
				stage('TEST2') {
					steps {
						sh 'sleep 5'
						echo "Testing Parallel"
					}
				}
				stage('TEST3') {
					steps {
						sh 'sleep 5'
						echo "Testing Parallel"
					}
				}
				stage('TEST4') {
					steps {
						sh 'sleep 5'
						echo "Testing Parallel"
					}
				}
			}	
		}
		
		stage('DEPLOY') {
			parallel {
				stage('AUTO') {
					steps {
						sh 'sleep 5'
						echo "Automation Testing"
					}
				}
				stage('Auto1) {
				      steps {
					      sh 'sleep 5'
					      echo "Automation Testing"
					}
				      }			         
			}
		}
	}
}
				
	



