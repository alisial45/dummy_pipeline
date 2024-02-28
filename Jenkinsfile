pipeline {
    agent any

    stages {
        stage('Name of Branch') {
            steps {
                script {
                    def branchName = ''
                    if (env.GITHUB_EVENT_NAME == 'push') {
                        def payload = readJSON text: env.CHANGE_PAYLOAD
                        branchName = payload.ref.split('/').last()
                    } else {
                        branchName = 'Branch name not available'
                    }
                    echo branchName
                }
            }
        }
    }
}
