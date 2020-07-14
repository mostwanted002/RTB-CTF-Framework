node {
	stage('Git checkout')
	{
		git credentialsId: 'mostwanted002', url: 'https://github.com/mostwanted002/RTB-CTF-Framework.git'
	}
	stage('Building docker images')
	{
	sh 'sudo docker-compose build'
	}
	stage('Spinning up')
	{
	sh 'sudo docker-compose up -d'
	}
}

//adding comment for trigger
