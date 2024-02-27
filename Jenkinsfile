pipeline {
    agent any
    stages {
        stage('Debug 0') {
    steps {
      script {
                    // Access the JSON payload of the webhook request
                    def payloadJson = env.JSON
                    
                    // Parse the JSON payload into a Groovy map
                    def payloadMap = readJSON text: payloadJson
                    
                    // Print specific information from the payload, such as the branch name
                    def branchName = payloadMap.ref
                    echo "Branch Name: $branchName"
                    
                    // Print the entire payload for debugging
                    echo "Webhook Payload: $payloadJson"
                }
    }
}
        
         stage('Debug') {
            steps {
                
                sh "echo 'Branch Name: ${env.BRANCH_NAME}'"
            }
        }
    }
}





