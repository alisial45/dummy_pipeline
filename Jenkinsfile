pipeline {
    agent any
    stages {
        stage('Debug 0') {
    steps {
        script {
            def payload = env.BUILD_CAUSE // Assuming BUILD_CAUSE contains the webhook payload
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





