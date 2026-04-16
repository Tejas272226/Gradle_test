pluggin{
	agent any
	
	tools{
		gradle 'Gradle'
		jdk 'JDK'
	}
	
	stages{
		stage('Checkout'){
			steps{
				git branch:'master',url:'https://github.com/Tejas272226/Gradle_test.git'
				}
			}
			
		stage('Build'){
				steps{
					sh 'gradle build'
					}
				}
			
		stage('Test'){
				steps{
					sh 'gradle test'
					}
				}
			
		stage('Run'){
			steps{
				sh 'gradle run'
				}
			}
		}
		
		post{
			success{
				echo 'Build and Deployment Successful!'
				}
			failure{
				echo 'Build Failed'
			}
		}
	}
	
