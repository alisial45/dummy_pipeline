  parameters {
        string(name: 'BRANCH_NAME', defaultValue: '', description: 'Name of the branch to build')
    }

    stages {
        stage('Hello') {
            steps {
                script {
                    // Get the branch name from the webhook payload
                    def branchNameFromPayload = "${env.GIT_BRANCH}" // Replace this with the code to extract the branch name from the payload
                    
                    // Set the default value of the BRANCH_NAME parameter
                    params.BRANCH_NAME = branchNameFromPayload
                    
                    echo "Building branch: ${params.BRANCH_NAME}"
                    // Add steps to build the specified branch
                }
            }
        }
    }
}

