pipeline {
    agent any

    parameters {
        string(name: 'GIT_BRANCH', defaultValue: 'master', description: 'Name of the branch to build')
    }
    
    stages {
        stage('Hello') {
            steps {
                script {
                    params.GIT_BRANCH = ${env.GIT_BRANCH}
                    def branchName = params.GIT_BRANCH
                    echo "Building branch: ${branchName}"
                    // Add steps to build the specified branch
                }
            }
        }
    }
    
}





