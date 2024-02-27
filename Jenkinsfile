pipeline {
    agent any
    stages {
        stage('Debug 0') {
    steps {
       script {
                    // Access the GitHub webhook event ID
                    def eventId = env.CHANGE_ID
                    
                    // Retrieve the full webhook payload using the event ID
                    def payload = httpRequest(url: "https://api.github.com/repos/alisial45/dummy_pipeline.git/hooks/${eventId}", authentication: 'dockerhub')
                    
                    // Print the webhook payload to the console
                    echo "Webhook Payload: $payload"
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





