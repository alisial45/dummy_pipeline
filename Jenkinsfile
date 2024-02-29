pipeline{
  agent any

  stages{

	  
    stage('checkout'){
			
echo env.GIT_BRANCH

	    checkout scmGit(
    branches: [[name: 'v4.11.x']],
    userRemoteConfigs: [[credentialsId:  'forwebhook',
        url: 'ssh://github.com:alisial45/dummy_pipeline.git']])
  }
		
  }
	
  
        
    }



