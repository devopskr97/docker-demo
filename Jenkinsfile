pipeline{
	agent { label 'docker'}
	stages{
		stage("docker image run"){
			script{
				sh " sudo docker ps "
			}
		}
	}
}
