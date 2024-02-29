pipeline{
  agent any

  stages{
    stage('checkout'){
			
	checkout scmGit(branches: [[name: 'origin/one-parameterized']],
                userRemoteConfigs: [
                    [ url: 'git@github.com:alisial45/dummy_pipeline.git' ]
                ])
  }
		
  }
  
        
    }



