pipeline{
	
	agent{
			docker{
			image 'maven'
			args '-v /root/apps/nexus--maven-samples:/root/.m2'
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
	
