pipeline{
	agent any
	stages{
		stage ('Compile Stage')
		{
			steps{
					bat 'call mvn clean compile'
			}
		}
		stage ('Test Stage'){
			steps{
					bat 'call mvn test'
			}
		}
		stage ('Package Stage'){
			steps{
					bat 'mvn package'
			}
		}
		stage ('Deployment Stage'){

			steps{
			    echo 'Deployed in this stage'
			}
		}
	}
}
