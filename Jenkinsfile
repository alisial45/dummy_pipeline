pipeline {
    agent any
    
    stages {
    
        stage('Checkout') {
            steps {
                // Checkout the selected branch
                script {
                    git branch: env.GIT_BRANCH, 
                        credentialsId: 'forwebhook', 
                        url: 'https://github.com/alisial45/dummy_pipeline.git'
                }
            }
        }
        
        // Other stages
    }
}


