pipeline{
  agent any

    stages {
      stage('Checkout') {
            steps {
                script {
                    // Get the branch name from the webhook payload
                    def branchNameFromPayload = env.GIT_BRANCH
                  
                

                  echo branchNameFromPayload
                  
                  
                
            }
        }
      
       stage('Hello') {
            steps {
               script {
    def branchNameFromPayload = env.GIT_BRANCH
    echo "Building branch: ${BRANCH_NAME}"
}
  }
        }
    }
}


