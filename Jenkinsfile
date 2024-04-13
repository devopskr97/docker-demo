pipeline{
	agent { label 'docker'}
	stages{
		stage("docker image run"){
			script{
				sh " sudo docker ps "
			}
		
		}
		stage ("Docker container run"){
			script{
				sh "sudo docker run -d -p 80:80 nginx"
			}
		}
	}
}
