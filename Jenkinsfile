pipeline{
	agent any
	stages{
		stage ('Compile Stage')
		{
			steps{
					echo 'mvn clean compile'
			}
		}
		stage ('Test Stage'){
			steps{
					echo 'mvn test'
			}
		}
		stage ('Package Stage'){
			steps{
					echo 'mvn package'
			}
		}
		stage ('Deployment Stage'){

			steps{
			    echo 'Deployed in this stage'
			}
		}
	}
}
