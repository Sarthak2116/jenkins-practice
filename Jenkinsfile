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
				withMaven(maven : 'maven-3-6-1'){
					sh 'mvn test'
				}
			}
		}
		stage ('Package Stage'){
			steps{
				withMaven(maven : 'maven-3-6-1'){
					sh 'mvn package'
				}
			}
		}
		stage ('Deployment Stage'){
			steps{
				withMaven(maven : 'maven-3-6-1'){
					sh 'mvn deploy'
				}
			}
		}
	}
}
