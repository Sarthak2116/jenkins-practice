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
					sh 'mvn test'
			}
		}
		stage ('Package Stage'){
			steps{
					sh 'mvn package'
			}
		}
		stage ('Deployment Stage'){

			steps{
			    sh 'echo Deployed in this stage'
			}
		}
	}
}
