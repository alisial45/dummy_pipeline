pipeline{
  agent any

  stages{
    stage('checkout'){
			
	checkout([
    $class: 'GitSCM',
    branches: [[name: 'origin/one-parameterized']],
    userRemoteConfigs: [[url: 'git@github.com:alisial45/dummy_pipeline.git']]
])

  }
		
  }
  
        
    }



