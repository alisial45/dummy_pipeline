pipeline{
  agent any

  stages{
    stage('checkout'){
			
			checkout scmGit(branches: [[name: 'stable-2.289']],
                userRemoteConfigs: [
                    [ url: 'git@github.com:alisial45/dummy_pipeline.git' ]
                ])
  }
		
  }
  
        
    }



