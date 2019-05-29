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
					sh 'mvn package'
			}
		}
		stage ('Deployment Stage'){

			steps{
			    sh 'git config --global user.email "sarthak321321@gmail.com"'
			    sh 'git config --global user.name "Sarthak2116"'
			    sh 'git config --global push.default simple'
			    sh('git push https://github.com/Sarthak2116/jenkins-practice.git')
			}
		}
	}
}
