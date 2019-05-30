pipeline{
	agent any
	stages{
		stage ('Compile Stage')
		{
			steps{
					sh 'mvn clean compile'
			}
		}
		stage ('Test Stage'){
			steps{
					sh 'mvn test'
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
