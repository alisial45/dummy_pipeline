pipeline{
  agent any

  stages{
    stage('checkout'){
			
echo env.GIT_BRANCH

	    checkout scmGit(
    branches: [[name: 'v4.11.x']],
    userRemoteConfigs: [[credentialsId:  'my-ssh-private-key-id',
        url: 'ssh://github.com/jenkinsci/git-plugin.git']])
  }
		
  }
	
  
        
    }



