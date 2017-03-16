node {
	stage ('SCM Update') {
			git credentialsId: 'svc-jenk', url: 'git@github.com:cmondor/ec-packer-poc.git'
	}

	stage ('build') {
		sh 'packer build packer.json'
	}
}