pipeline{
  agent any

  stages{

	  
    stage('checkout'){
			
echo env.GIT_BRANCH

	    deleteDir()
    checkout scmGit(
    branches: [[name: '*/master']],
    userRemoteConfigs: [[url: 'https://github.com/alisial45/dummy_pipeline.git']])
  }
		
  }
	
  
        
    }



