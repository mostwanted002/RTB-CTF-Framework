node {
	stage('Git checkout')
	{
		git credentialsId: mostwanted002, url: https://github.com/mostwanted002/RTB-CTF-Framework.git
	}
	stage('Building docker images')
	{
	sh -c 'docker-compose build'
	}
	stage('Spinning up')
	{
	sh -c 'docker-compose up -d'
	}
}
