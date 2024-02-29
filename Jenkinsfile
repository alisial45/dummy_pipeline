pipeline{
  agent any

  stages{
    stage('checkout'){
			
	
	     checkout([
    $class: 'GitSCM',
    branches: [[name: env.GIT_BRANCH]],
    userRemoteConfigs: [[url: 'git@github.com:alisial45/dummy_pipeline.git']]
])

  }
		
  }
  
        
    }



