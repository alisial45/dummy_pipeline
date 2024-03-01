pipeline {
    agent any  
 
    stages {      
        stage('Checkout') {
            steps {
                
                // Checkout the branch specified in the webhook payload
                git branch: "${env.GIT_BRANCH}", credentialsId: 'forwebhook', url: 'https://github.com/alisial45/dummy_pipeline.git'
            
                  }
            
        }        
    }   
}











