node{
    stage('Git Checkout'){
        git credentialsId: 'github-credentials', url: 'https://github.com/yogeshdewangan/fiboweb'
    }
	
	stage('Build images'){
		client = docker.build("yogeshdewangan97/client")
		server = docker.build("yogeshdewangan97/server")
		worker = docker.build("yogeshdewangan/workder")
		
	}
}

