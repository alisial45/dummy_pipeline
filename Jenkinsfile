pipeline {
    agent any
    stages {
        stage('Debug 0') {
    steps {
     script {
                    echo "Webhook Payload: ${env.JSON}"
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





