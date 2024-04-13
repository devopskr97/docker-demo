pipeline{
	agent { label 'docker'}
	stages{
		stage("git checkout"){
			steps{
				script{
					git 'https://github.com/devopskr97/docker-demo.git' 
				}
			}	
		
		}
		stage ("Docker image Build"){
			steps{
				script{
					sh "sudo docker build -t demo ."
				}
			}
		}
		stage ("Docker run container"){
			steps{
				script{
					sh "sudo docker run -d -p 5000:5000 demo"
				}
			}
		}
		stage ("Docker container status"){
			steps{
				Script{
					sh "sudo docker ps"
				}
			}
		}
	}
  }
