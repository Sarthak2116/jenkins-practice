pipeline{
	agent any
	stages{
		stage ('Compile Stage')
		{
			steps{
					sh 'call mvn clean compile'
			}
		}
		stage ('Test Stage'){
			steps{
					sh 'call mvn test'
			}
		}
		stage ('Package Stage'){
			steps{
					sh 'call mvn package'
			}
		}
		stage ('Deployment Stage'){

			steps{
			    echo 'Deployed in this stage'
			}
		}
	}
}
