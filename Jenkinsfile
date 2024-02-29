pipeline{
  agent any

    stages {
        stage('Hello') {
            steps {
               script {
    // Get the branch name from the webhook payload
    def branchNameFromPayload = env.GIT_BRANCH
    
    // Set the default value of the BRANCH_NAME parameter
    def BRANCH_NAME = branchNameFromPayload
    
    echo "Building branch: ${BRANCH_NAME}"
    // Add steps to build the specified branch
}
            }
        }
    }
}

