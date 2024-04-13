pipeline{
	agent { label 'docker'}
	stages{
		stage("docker image run"){
			steps{
				script{
					sh " sudo docker ps "
				}
			}	
		
		}
		stage ("Docker container run"){
			steps{
				script{
					sh "sudo docker build -t demo ."
				}
			}
		}
	}
	}
