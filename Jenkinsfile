pipeline{
	
	agent{
		docker{
			image 'maven'
			args '-v /root/apps/nexus/Mavendeploy:/root/.m2'
			}
        }
		stages{
			
			stage('deploy'){
				steps{
					script{
						sh "mvn clean deploy"
						}
					}
				}
			}
}
	
