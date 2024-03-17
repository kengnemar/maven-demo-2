pipeline{
	agent any
	stages{
		stage("Clone Code from the GitHub Repo"){
			steps{
				git credentialsId: 'git_credentials', url: 'https://github.com/kengnemar/maven-demo-2'
			}
		}
		stage("Build Artifact"){
			steps{
				sh "mvn clean install"
				}
		}
	}
}

