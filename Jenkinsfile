pipeline {
    agent any

    parameters {
        
        string(name: 'GIT_BRANCH', defaultValue: 'master', description: 'Name of the branch to build')
    }
    stages {
        stage('Fetch Branch') {
            steps {
                echo "Fetching branch: ${env.GIT_BRANCH}"
                // Add steps to fetch and checkout the specified branch
                git branch: "${env.GIT_BRANCH}", url: 'https://github.com/alisial45/dummy_pipeline.git'
            }
        }
    }
    
}










