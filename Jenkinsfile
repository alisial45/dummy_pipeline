pipeline {
    agent any
    
    parameters {
        string(name: 'BRANCH_TO_BUILD', defaultValue: '', description: 'Enter the branch to build')
    }
    
    stages {
        stage('Checkout') {
            steps {
                script {
                    // Use the specified branch or fallback to GIT_BRANCH if not provided
                    def branchName = params.BRANCH_TO_BUILD ?: env.GIT_BRANCH
                    git branch: branchName, credentialsId: 'your-git-credentials-id', url: 'https://github.com/alisial45/dummy_pipeline.git'
                }
            }
            
        }
        
        // Other stages
    }
}



