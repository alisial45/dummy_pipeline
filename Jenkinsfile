pipeline {
    agent any
    
    parameters {
        // Define Git parameter to select branch dynamically
        gitParameter(branch: '', 
                     defaultValue: env.GIT_BRANCH, 
                     description: 'Select the branch to build')
    }

    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the selected branch
                script {
                    git branch: "${params.BRANCH_TO_BUILD}", 
                        credentialsId: 'forwebhook', 
                        url: 'https://github.com/alisial45/dummy_pipeline.git'
                }
            }
        }
        
        // Other stages
    }
}
