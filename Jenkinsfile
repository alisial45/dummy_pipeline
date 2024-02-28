pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script {
                    def branchName = env.GIT_BRANCH ?: 'Branch name not available'
                    echo "Branch Name: ${branchName}"
                }
            }
        }
    }
}
