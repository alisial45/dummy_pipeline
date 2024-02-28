pipeline {
    agent any

    stages {
        stage('Payload') {
            steps {
                script {
                    def payload = env.CHANGE_PAYLOAD ?: 'No payload available'
                    echo "Webhook Payload: ${payload}"
                }
            }
        }
    }
}
