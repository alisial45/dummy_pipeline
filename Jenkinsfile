pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                script {
                    def branchName = ${env.GIT_BRANCH}
                    echo "Building branch: ${branchName}"
                    // Add steps to build the specified branch
                }
            }
        }
    }
}


