pipeline {
    agent any
    stages {
        stage('Debug 0') {
    steps {
       script {
                    def payload = change
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





